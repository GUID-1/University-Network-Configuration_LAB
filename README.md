# University-Network-Configuration_LAB
Configuring a university network topology utilizing the the following: Switchport modes, VLANS, DHCP, Sub-interfaces, Routing Protocols (OSPF) &amp; Router-On-A-Stick

<h1>University Network Packet Tracer Home Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/2eN5QdSPeBk)

<h2>Description</h2>
Project consists of a University Network that incorporates the configuration of DHCP, VLANS, 802.1Q encapsulation, access point, OSPF, rotuer-on-a-stick & static IP addressing  
<br />


<h2>Languages and Utilities Used</h2>

- <b>Cisco CLI</b> 

<h2>Environments Used </h2>

- <b>Packet Tracer 9.0</b> 

<h2>Configuration walk-through:</h2>

<p align="center">
VLAN configuration: <br/>
<img src="https://www.image2url.com/r2/default/images/1788313780814-1e888172-9a0d-4f15-9af0-40129356d8f4.png" alt="Vlan Config Steps" />
<br />
<br />
Switchport Access Config:  <br/>
<img src="https://www.image2url.com/r2/default/images/1788317218312-b8258876-8c00-477d-9569-9f451638eb29.png" alt="Switchport Access Config Steps" />
<br />
<br />
Switchport Access Config: <br/>
<img src="https://www.image2url.com/r2/default/images/1788317969341-d070d81b-7573-40fe-a084-e0eccf09af29.png" alt="Switchport Access Config Steps Con't" />
<br />
<br />
Router Subinterface Configuration:  <br/>
<img src="https://www.image2url.com/r2/default/images/1788319329643-999dffca-61ae-4899-b9e2-c374250e49a1.png" alt="Router Configuration Steps" />
<br />
<br />
Router Subinterface Configuration (continued):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788319519484-442844d6-1e86-4119-a98e-c958deccb4e2.png" alt="Router Configuration Steps" />
<br />
<br />
Router Subinterface Configuration (continued):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788339247988-1230d506-da28-4967-bbf0-9eb8329735bc.png" alt="Router Configuration Steps" />
 Add a /26 subnet mask for the ip addr 192.168.1.129
<br />
<br />
Router DHCP Configuration:  <br/>
<img src="https://www.image2url.com/r2/default/images/1788346272982-4b5f063a-fedd-4979-943a-7cf38bb07b56.png" alt="DHCP Configuration" />
<br />
<br />
Router DHCP Configuration (continued):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788346830053-c6b86169-a53c-4d7f-83fb-4310281591a2.png" alt="DHCP Configuration" />
<br />
<br />
SSH Configuration:  <br/>
<img src="https://www.image2url.com/r2/default/images/1788347531109-e5c47e6f-b3a1-4bdb-b511-8fbfe9fa8403.png" alt="SSH Configuration" />
<br />
<br />
SSH Configuration (continued):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788348028844-86682d2d-b682-4d34-be58-ea4e721a4a1d.png" alt="SSH Configuration" />
<br />
<br />
SSH Configuration (continued):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788349472605-c13fbd5b-2431-4417-87d9-9da06f715b92.png" alt="SSH Configuration" />
<br />
<br />
SSH Configuration (continued):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788350016099-1ce015ef-356d-4a32-b3e0-c64d41dcae23.png" alt="SSH Configuration" />
<br />
<br />
  SOP: Configure a Router-on-a-Stick Network with VLANs, DHCP, Wireless Access, and SSH

### Objective

Set up a small office/home office network using VLAN segmentation on a switch, router-on-a-stick inter-VLAN routing, DHCP for client addressing, wireless access for a laptop, and secure SSH management access to the router. This SOP ensures devices in the same VLAN can communicate, devices in different VLANs can route through the router, and the router can be managed securely.

### Key Steps

**1. Create and verify VLANs on the switch** 

- Enter switch CLI configuration mode.
- Create the required VLANs: 
  - VLAN 10 for Sales
  - VLAN 20 for IT
  - VLAN 30 for HR
- Assign clear names to each VLAN so the department purpose is obvious.
- Run `show vlan` to confirm the VLANs were created successfully.
- Use VLANs to segment the network by department and control communication paths.

**2. Assign switch ports to the correct access VLANs** 

- Identify which switch ports connect to each end device.
- Use `interface range` to configure multiple ports at once.
- Set end-device ports to **access mode**.
- Assign ports to the correct VLANs: 
  - Sales devices to VLAN 10
  - IT devices to VLAN 20
  - HR devices to VLAN 30
- Recheck with `show vlan` to verify ports appear under the correct VLANs.
- Keep the port-to-VLAN mapping documented for troubleshooting.

**3. Configure static IP addresses for end devices within each VLAN** 

- Open each PC or device and go to the IP configuration screen.
- Assign a static IP address that matches the device’s VLAN subnet.
- Use the same subnet mask for all devices in the same VLAN.
- Keep devices in the same VLAN within the same broadcast domain.
- Example approach used in the demo: 
  - Sales devices in the 192.168.1.0/26 network
  - IT devices in the 192.168.1.64/26 network
  - HR devices in the 192.168.1.128/26 network
- Test local connectivity by pinging devices within the same VLAN.

**4. Confirm intra-VLAN communication before enabling inter-VLAN routing** 

- Ping devices within the same VLAN to confirm local switching works.
- Verify that packets stay within the VLAN and reach the correct end device.
- If same-VLAN pings fail, check: 
  - VLAN assignment on the switch
  - Access mode configuration
  - IP address and subnet mask consistency
- Do not move to router configuration until same-VLAN communication is working.

**5. Bring up the router interface for the trunk link** 

- Enter the router CLI.
- Go to the physical interface connected to the switch, such as `g0/1`.
- Use `no shutdown` to enable the interface.
- Confirm link lights or interface status show the connection is active.
- If the link is still down, verify cabling and switch-side trunk configuration.

**6. Configure router subinterfaces for router-on-a-stick** 

- Create one subinterface per VLAN on the router.
- Match each subinterface number to the VLAN ID for clarity: 
  - `g0/1.10` for VLAN 10
  - `g0/1.20` for VLAN 20
  - `g0/1.30` for VLAN 30
- Apply 802.1Q encapsulation to each subinterface.
- Assign the default gateway IP address for each VLAN subnet: 
  - VLAN 10 gateway: 192.168.1.1
  - VLAN 20 gateway: 192.168.1.65
  - VLAN 30 gateway: 192.168.1.129
- Add descriptions to each subinterface for easier troubleshooting.
- Save the configuration and verify with `show run`.

**7. Configure DHCP pools on the router for each VLAN** 

- Enable DHCP service on the router.
- Create a DHCP pool for each VLAN.
- For each pool, define: 
  - Network address
  - Subnet mask
  - Default router (gateway)
  - DNS server
  - Optional domain name
- Example pools from the demo: 
  - Sales: 192.168.1.0/26, gateway 192.168.1.1
  - IT: 192.168.1.64/26, gateway 192.168.1.65
  - HR: 192.168.1.128/26, gateway 192.168.1.129
- Verify the DHCP pools with `show run` or the DHCP pool display command.
- Ensure the router’s gateway IPs match the subinterface addresses exactly.

**8. Configure the access point and wireless client** 

- Configure the access point with an SSID.
- Set wireless authentication and a password.
- Connect the laptop to the wireless network using the correct SSID and password.
- Assign the access point a static IP address in the appropriate VLAN subnet.
- Confirm the wireless client receives the correct gateway and DNS settings if DHCP is used.
- Test wireless connectivity by pinging a device in the same VLAN.

**9. Test inter-VLAN routing and DHCP assignment** 

- Change end devices from static IPs to DHCP where appropriate.
- Confirm each device receives: 
  - IP address
  - Subnet mask
  - Default gateway
  - DNS server
- Test communication between devices in different VLANs.
- If inter-VLAN pings fail, check: 
  - Router subinterfaces
  - VLAN-to-subinterface mapping
  - DHCP pool settings
  - Default gateway values
- Confirm that devices in different VLANs can now communicate through the router.

**10. Secure router management with SSH** 

- Assign a hostname to the router.
- Configure an IP domain name.
- Create a local username and password.
- Generate RSA crypto keys with a 1024-bit key size.
- Enable SSH version 2.
- Configure VTY lines to accept SSH only.
- Set `login local` so the router uses the local user database.
- Add an enable password so privileged mode access is protected.
- Assign a management IP address to the router that does not conflict with existing subnets.

**11. Validate SSH access from a client device** 

- From a client PC, open an SSH session to the router’s management IP.
- Log in using the configured username and password.
- Enter the enable password when prompted.
- Confirm you can reach privileged EXEC mode and configuration mode.
- If login fails, verify: 
  - SSH version and keys
  - VTY line settings
  - Username/password
  - Management IP address
  - Network reachability

### Cautionary Notes

- Ensure each VLAN uses a unique subnet and that no IP addresses overlap.
- Do not forget to enable the router interface with `no shutdown`.
- Trunking must be configured correctly between the switch and router for router-on-a-stick to work.
- Static IPs are useful for infrastructure devices like printers and access points; DHCP is better for most user devices.
- The first ping to a new destination may fail due to ARP resolution; test more than once before assuming failure.
- SSH requires a hostname, domain name, RSA keys, and VTY configuration; missing any of these can prevent access.
- Avoid using Telnet for management unless absolutely necessary, since it is not secure.

### Tips for Efficiency

- Plan the VLANs, subnets, and gateway addresses on paper before configuring devices.
- Use `interface range` on the switch to configure multiple ports faster.
- Keep a consistent naming convention for VLANs, subinterfaces, and DHCP pools.
- Add descriptions to interfaces and subinterfaces to simplify troubleshooting later.
- Verify each stage before moving on: VLANs, access ports, routing, DHCP, wireless, then SSH.
- Save configurations after major changes to avoid losing work.
- Use DHCP for end-user devices to reduce manual configuration time and errors.

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
