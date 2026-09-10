# University-Network-Configuration_LAB
Configuring a university network topology utilizing the the following: Switchport modes, VLANS, DHCP, Sub-interfaces, Routing Protocols (OSPF) &amp; Router-On-A-Stick

<h1>University Network Packet Tracer Home Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/2eN5QdSPeBk)

<h2>Description</h2>
Project consists of a University Network that incorporates the configuration of DHCP, VLANS, 802.1Q encapsulation, access point, OSPF, rotuer-on-a-stick & static IP addressing  
<br />


<h2>Languages and Utilities Used</h2>

- <b>Cisco CLI</b>

<h2>Cisco CLI Commands Used</h2>

- <b>Enable (en)</b>
- <b>Configure Terminal (conf t)</b>
- <b>Do Show Vlan (do sh vlan)</b>
- <b>Do Show Interfaces Status (do sh interfaces status)</b>
- <b>Interface Range (int range)</b>
- <b>Switchport Mode Access (sw mod acc)</b>
- <b>Switchport Access vlan (sw acc vlan)b>
- <b>Do Write (do wr)</b>
- <b>Do Show Run (do sh run)</b>
- <b>Switchport Mode Trunk (sw mod trunk)</b>
- <b>Do Show Controllers Serial (do sh controll se)</b>
- <b>Clock Rate(clock ra)</b>
- <b>Service DHCP (service dhc)</b>
- <b>IP DHCP Pool (ip dhcp pool)</b>
- <b>Network (netwo)</b>
- <b>Default-Router (defaul)</b>
- <b>DNS-Server (dns)</b>
- <b>Domain-Name (domai)</b>
- <b>Encapsulation Dot1q (encap dot)</b>
- <b>CDP Run (cdp run)</b>
- <b>Do Show CDP Neighbor (do sh cdp neighb)</b>
- <b>Do Show CDP Neighbor Detail (do sh cdp neighbor det)</b>
- <b>Do Show IP Interface Brief (do sh ip int bri)</b>
- <b>Router OSPF (router os)</b>
- <b>Do Show IP Route (do sh ip rout)</b>
- <b>Do Show IP Route OSPF (do sh ip rout ri)</b>

<h2>Environments Used </h2>

- <b>Packet Tracer 9.0</b> 

<h2>Configuration walk-through:</h2>

<p align="center">
VLAN configuration (SW-1 ADMIN): <br/>
<img src="https://www.image2url.com/r2/default/images/1788938923719-1a66d3f8-7d2e-449a-a951-5e2d08687a06.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-2 HR):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788940559890-98137842-f8af-4807-8c40-7f1953a84a63.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-3 FINANCE):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788940732849-a19fe9c7-d771-4e29-928c-1c0a43dfb0c7.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-4 BUSINESS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788943783306-c8680160-2652-4316-a18b-f4c78048ad3b.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-5 ENERGY):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946181422-4e0b92c5-7c49-4cc7-802b-0a86cfdf0cde.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-6 ART&DESIGN):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788944112688-9416a806-55fa-4a98-8092-833e0aa1979f.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-7 STD-LABS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788945936280-f350bccc-3965-492f-8acd-c747b5805a08.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-8 IT):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946468168-bd0223f6-5877-4729-81c6-4f7de6c2e47b.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-9 STAFF):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946694336-2165a477-0253-4d0a-8804-01b07937523c.png" alt="VLAN Configuration" />
<br />
<br />
VLAN configuration (SW-10 STD-LABS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946863382-7f8f48af-f5ae-49cb-b3f3-260190b70e3f.png" alt="VLAN Configuration" />
<br />
<br />
VLAN & Switchport configuration (L3-SW MAIN-CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788349472605-c13fbd5b-2431-4417-87d9-9da06f715b92.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1788953237741-2d1477ef-c223-4b68-b57e-fe2eebae6501.png" alt="Switchport Trunk" />
<br />
<br />
Router configuration (R1 MAIN-CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788953953565-36a432d1-ab74-46a3-bfa3-78d9519211f7.png" alt="DHCP Service" />
<img src="https://www.image2url.com/r2/default/images/1788954205662-b27e6825-c44c-4f3e-bbb1-b859f645db13.png" alt="Interface Activation" />
<img src="https://www.image2url.com/r2/default/images/1788954366813-3f3311ed-ac20-4c80-bb1e-2b7eff9e5e38.png" alt="Interface Activation" />
<br />
<br />
Router configuration (R2 BRANCH-CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788953658052-51a02771-596f-4a74-92b4-df4ccdfc88a9.png" alt="Switchport Configuration" />
<img src="https://www.image2url.com/r2/default/images/1788954475657-e6ab5100-e6ca-4085-940b-af178d64e8be.png" alt="Interface Activation" />
<br />
<br />
Router configuration (R3 CLOUD):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788954880301-f069ffda-53fe-4011-9f74-b69bdc9b222a.png" alt="Interface Activation" />
<img src="https://www.image2url.com/r2/default/images/1788954475657-e6ab5100-e6ca-4085-940b-af178d64e8be.png" alt="Interface Activation" />
<br />
<br />
CDP configuration (SW-1-10, L3-SW, Routers): <br/>
<img src="https://www.image2url.com/r2/default/images/1789000755020-7c808998-61a2-47c7-afb4-f97342176085.png" alt="CDP Enable" />
 -This command can be used on every networking device to configure and enable CDP
<br />
<br />
CDP Interface Disable (SW-2 HR):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789001629222-9eee7746-9be8-4cb4-abf7-dc502e971dfb.png" alt="CDP Disable" />
-Disabling CDP on interfaces connected to end devices increases security
-Discover which interfaces are connected to end devices and input the command listed to disable CDP (no cdp enable)
<br />
<br />
Router Clock Rate Configuration (R1 MAIN_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789002396959-37b61705-bde4-4416-b584-13a5a320f91c.png" alt="Clock Rate Configuration" />
<br />
<br />
Router DHCP Configuration (R1 MAIN_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789003154283-b2dd4a56-cae5-4417-bedf-c4bb379691d0.png" alt="DHCP Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789003290277-2638847c-0671-4fb1-b7cf-99f528b33bc9.png" alt="DHCP Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789003400309-a41aed58-08de-43eb-af1f-2c5389f2310c.png" alt="DHCP Configuration" />
<br />
<br />
Router DHCP & Sub-interface Configuration (R2 BRANCH_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789003648353-aed4e60a-7798-4139-ac2c-b82ab43fa3aa.png" alt="DHCP Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789003765441-c4466cdb-14c7-479b-8e5c-d6ab3ce92fd9.png" alt="DHCP Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789004066432-5fd4bd20-f255-4b12-9776-6e8c9f97b783.png" alt="Sub-Interface Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789004189879-c7f04e89-0852-4272-b768-fd37070e6243.png" alt="Sub-Interface Configuration" />
<br />
<br />
CDP configuration (SW-6 ART&DESIGN):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788944112688-9416a806-55fa-4a98-8092-833e0aa1979f.png" alt="VLAN Configuration" />
<br />
<br />
CDP configuration (SW-7 STD-LABS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788945936280-f350bccc-3965-492f-8acd-c747b5805a08.png" alt="VLAN Configuration" />
<br />
<br />
CDP configuration (SW-8 IT):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946468168-bd0223f6-5877-4729-81c6-4f7de6c2e47b.png" alt="VLAN Configuration" />
<br />
<br />
CDP configuration (SW-9 STAFF):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946694336-2165a477-0253-4d0a-8804-01b07937523c.png" alt="VLAN Configuration" />
<br />
<br />
CDP configuration (SW-10 STD-LABS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1788946863382-7f8f48af-f5ae-49cb-b3f3-260190b70e3f.png" alt="VLAN Configuration" />
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
