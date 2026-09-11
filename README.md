# University-Network-Configuration_LAB
Configuring a university network topology utilizing the the following: Switchport modes, VLANS, DHCP, Sub-interfaces, Routing Protocols (OSPF) &amp; Router-On-A-Stick

<h1>University Network Packet Tracer Home Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/WC-J1E3Ai3g)

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
<img src="https://www.image2url.com/r2/default/images/1789008893008-6bb9e91f-35a9-4764-ab5a-8d4c369edbd7.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789008990878-c763a9de-5947-42fa-88a1-e5def5227dd3.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789009103587-c3e7d6e6-0d45-4fe0-8d4c-4c544f0fd0e0.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789009223061-5269e2d5-2e92-4de4-b52c-bb93e57a6e24.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789009309927-7f528703-7e44-4cd7-b129-6f617a1e79e2.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1788953237741-2d1477ef-c223-4b68-b57e-fe2eebae6501.png" alt="Switchport Trunk" />
<br />
<br />
VLAN configuration (L3-SW BRANCH-CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789009745285-0e8e4e74-ce60-41cb-b761-ec36a58c9dd1.png" alt="VLAN Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789009819738-7b39292c-d6ce-4d56-86e5-8f6ba6d7c5bb.png" alt="VLAN Configuration" />
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
Router Sub-interface Configuration (R1 MAIN_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789004616737-4a928c44-e613-4f03-8d7e-48e65b38236b.png" alt="Sub-Interface Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789004723389-8430c757-ae58-457c-a93b-fe9304bcc48e.png" alt="Sub-Interface Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789004951909-07148d80-a47e-4eb9-855a-32783de0067a.png" alt="Sub-Interface Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789005293008-7a7c92d5-94ac-4248-a5e0-6b535a447882.png" alt="Sub-Interface Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789005386468-86015b29-6c58-4d0a-891a-2ecdd0799679.png" alt="Sub-Interface Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789005469994-4c9fbd09-e3c9-423e-9b6e-6c14f99a1557.png" alt="Sub-Interface Configuration" />
<br />
<br />
Static IP Configuration (WEB-SERVER):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789005942793-cf0e22c6-339f-4788-9405-f7a0fc6d9189.png" alt="Static IP Configuration" />
<br />
<br />
Static IP Configuration (FTP-SERVER):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789006052930-7986d840-9e0e-4ade-a192-e47e2e892754.png" alt="Static IP Configuration" />
<br />
<br />
Router IP Address Configuration (R1 MAIN_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789006799590-1a0397fc-b7b4-40c7-94fa-ca48975fb428.png" alt="IP Address Configuration" />
<br />
<br />
Router IP Address Configuration (R2 BRANCH_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789007019212-658c4b91-5154-4543-99db-42191868126a.png" alt="IP Address Configuration" />
<br />
<br />
Router IP Address Configuration (R3 CLOUD):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789007174975-f61fbf64-1ccf-47cb-b924-5cecea198700.png" alt="IP Address Configuration" />
<br />
<br />
Static IP Configuration (FTP-SERVER): 
<img src="https://www.image2url.com/r2/default/images/1789007351394-111f51b7-fce6-4c2a-a27a-4e3c7cb36995.png" alt="Static IP Configuration" />
<br />
<br />
Router Routing Protocol Configuration (R2 BRANCH_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789007563085-8a4c1ce9-558f-4d77-892e-d82037d20a87.png" alt="OSPF Configuration" />
<img src="https://www.image2url.com/r2/default/images/1789007699356-638d828f-a0a8-4851-af80-fbcb1785abb3.png" alt="OSPF Configuration" />
<br />
<br />
Router Routing Protocol Configuration (R1 MAIN_CAMPUS):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789008034661-3f6fec9d-c989-441a-8132-30ee013e0d65.png" alt="OSPF Configuration" />
<br />
<br />
Router Routing Protocol Configuration (R3 CLOUD):  <br/>
<img src="https://www.image2url.com/r2/default/images/1789008154665-bb391918-e6c8-4de8-8b53-46628917dc2f.png" alt="OSPF Configuration" />
<br />
<br />
 
## SOP: Configure a University Network Topology with VLANs, DHCP, Router-on-a-Stick, and OSPF

### Objective

Configure and verify a multi-department university network by assigning VLANs, enabling DHCP, setting up router-on-a-stick subinterfaces, and advertising routes with OSPF so all departments can communicate across the network.

### Key Steps

**1. Label and prepare the access-layer switches** [0:40]

- Start with **Switch 1** and label it according to the department it serves.
- Continue through each access switch in a **linear, one-switch-at-a-time** method.
- Keep a consistent naming convention so each switch can be identified quickly during troubleshooting.
- Verify the switch name and role before applying any configuration.

 

**2. Configure VLAN 10 for the Admin department** [1:08]

- Enter configuration mode on the first switch.
- Use an **interface range** command to place all end-device ports into **access mode**.
- Include the uplink interface connected to the Layer 3 switch if it is being assigned to the same VLAN.
- Create **VLAN 10** and name it **Admin**.
- Run `show vlan` to confirm the ports are assigned correctly.

 

**3. Configure VLAN 20 for the HR department** [1:57]

- Move to **Switch 2** and repeat the same access-port procedure.
- Place the relevant interfaces into **access mode**.
- Create **VLAN 20** and name it **HR**.
- Verify the VLAN assignment with `show vlan` before moving to the next switch.

 

**4. Configure VLAN 30 for the Finance department** [2:41]

- On the next switch, enter configuration mode.
- Use the same interface-range approach to assign ports to access mode.
- Create **VLAN 30** and name it **Finance**.
- Confirm the VLAN membership with `show vlan`.

 

**5. Configure VLAN 40 for the Business department** [3:18]

- Configure the next switch using the same repeatable process.
- Set the selected interfaces to **switchport mode access**.
- Assign them to **VLAN 40**.
- Name the VLAN **Business**.
- Check the result with `show vlan`.

 

**6. Configure VLAN 50 for the next department switch** [3:53]

- Continue to the next access switch.
- Use the same interface-range and access-mode configuration.
- Assign the ports to **VLAN 50**.
- Apply the department name consistently.
- Save the configuration after verifying the VLAN assignment.

 

**7. Configure VLAN 60 for the Art and Design department** [4:46]

- Move to the **Art and Design** switch.
- Put all end-device ports into **access mode**.
- Assign the interfaces to **VLAN 60**.
- Name the VLAN **Art and Design**.
- Verify with `show vlan`.

 

**8. Configure VLAN 70 for the Student Lab department** [5:42]

- On the **Student Lab** switch, enter configuration mode.
- Use the same interface-range procedure.
- Set the ports to **access mode** and assign them to **VLAN 70**.
- Name the VLAN **Student Lab**.
- Confirm the configuration with `show vlan`.

 

**9. Configure VLAN 80 for the IT department** [6:29]

- On the **IT department** switch, repeat the same access-layer configuration.
- Assign the interfaces to **VLAN 80**.
- Name the VLAN **IT department**.
- Use `show vlan` to verify the ports and VLAN name.

 

**10. Enable CDP and document configuration practices** [7:02]

- Consider using a text editor or notes file to prepare commands before entering them on devices.
- Copying commands from a prepared document can reduce typing errors and speed up deployment.
- Use this method carefully and still verify each command on the device.
- Keep the same naming and configuration standards across all switches.

 

**11. Configure the Layer 3 campus switch and resolve VLAN mismatches** [8:46]

- Move to the **main campus Layer 3 switch**.
- Review mismatch messages shown on the terminal to identify unconfigured interfaces.
- Configure each interface in **access mode** and assign it to the correct VLAN.
- Match the access mode on both sides of the connection.
- Continue using the same naming conventions used on the access switches.

 

**12. Finish Layer 3 switch VLAN assignments and verify** [11:14]

- Continue configuring the remaining Layer 3 switch interfaces.
- Assign each interface to the correct VLAN based on the department mapping.
- Watch mismatch messages decrease as configuration is completed.
- Use `show vlan` to confirm VLANs 10, 20, 30, 40, 50, 60, 70, and 80 are present with the correct interfaces.

 

**13. Configure the branch Layer 3 switch VLANs** [14:52]

- Move to the **branch campus Layer 3 switch**.
- Configure only the VLANs needed for that site.
- Assign the first interface to **VLAN 100** and the second to **VLAN 90**.
- Use access mode for both interfaces.
- Verify the result with `show vlan`.

 

**14. Enable DHCP on the main campus router and set the uplink to trunk** [16:19]

- Go to the **main campus router**.
- Enable the **DHCP service** so the router can assign IP addresses to clients.
- Configure the router-facing switch port as a **trunk** where required.
- Use `show run | include trunk` to confirm trunk configuration.
- Bring interfaces up with `no shutdown` if needed.

 

**15. Bring up router and switch interfaces and enable CDP** [21:06]

- Check whether interfaces are administratively down.
- Use `no shutdown` on the router interfaces to bring them online.
- Repeat the process on the **branch router** and any other connected routers.
- Enable **CDP** on switches, routers, and Layer 3 devices where discovery is desired.
- Disable CDP on end-device-facing ports if information exposure is a concern.

 

**16. Verify CDP neighbors and configure serial clock rate** [29:00]

- Run `show cdp neighbors` to confirm connected devices and interfaces.
- Review the neighbor table to validate topology visibility.
- On serial DCE interfaces, configure the **clock rate**.
- Use the recommended clock rate of **64000** when applicable.
- Verify the serial interface status after configuration.

 

**17. Create DHCP pools on the main campus router** [32:11]

- Enter DHCP pool configuration mode on the main campus router.
- Create a pool for each department subnet.
- Use the correct **network address**, **default router**, and **DNS server** values.
- Follow the naming convention: department name followed by `.com`.
- Use the first usable IP address in each subnet as the default gateway and DNS server reference.

 
**18. Document DHCP design rules and save the configuration** [34:38]

- Reserve static IP addresses for devices like printers, web servers, and FTP servers.
- Use DHCP for client devices that need dynamic addressing.
- Keep address allocation organized so troubleshooting is easier.
- Run `show run | include dhcp` to confirm pool settings.
- Save the configuration with `write` or the equivalent save command.

 

**19. Configure DHCP pools on the branch campus router** [39:13]

- Enable DHCP on the **branch campus router**.
- Create the required pools for the branch subnets.
- Use the same DHCP structure and naming conventions as the main campus router.
- Double-check the network statements and pool names before saving.
- Verify the configuration after completion.

 

**20. Configure router-on-a-stick subinterfaces for VLAN routing** [42:06]

- On the router connected to the Layer 3 switch, create **subinterfaces**.
- Use the subinterface number to match the VLAN number.
- Apply **802.1Q encapsulation** with the correct VLAN ID.
- Assign the subinterface the **default router IP address** for that subnet.
- Add a short description to identify the department or VLAN.

 

**21. Complete subinterface configuration for all campus VLANs** [45:04]

- Repeat the subinterface process for VLANs **10, 20, 30, 40, 50, 60, 70, and 80**.
- Ensure each subinterface uses the correct VLAN tag and gateway IP.
- Use `show ip interface brief` to confirm the subinterfaces are up and have IP addresses.
- Compare the subinterface list against the DHCP pool settings to ensure consistency.

 

**22. Test DHCP assignment on end devices and configure static servers** [51:06]

- On client devices, request a DHCP address and confirm the lease is successful.
- Repeat the test on multiple end devices across departments.
- Configure the **web server** with a static IP address and set the correct default gateway and DNS server.
- Configure the **FTP server** with a static IP address in the same subnet.
- Ensure static addresses do not conflict with DHCP assignments.

 

**23. Test interdepartmental connectivity and identify routing gaps** [55:01]

- Ping devices in other subnets to confirm cross-network communication.
- Expect the first ping to time out in some cases, then retry.
- If packets fail to reach remote subnets, check routing configuration.
- Confirm whether routing protocols and router IP addresses are fully configured.
- Use ping results to identify which networks are reachable and which are not.

 

**24. Configure router IP addresses on serial links** [57:51]

- Assign IP addresses to the serial interfaces between routers.
- Use a **/30 subnet** for point-to-point links.
- Configure the main campus router, branch router, and cloud router interfaces with matching subnet pairs.
- Bring the interfaces up and verify they are connected.
- Check interface status to confirm the serial links are operational.

 

**25. Configure OSPF on the branch router** [01:03:25]

- Enable **OSPF** with process ID **1**.
- Advertise the branch router’s connected networks.
- Use the correct wildcard mask for each subnet.
- Verify that the router learns and advertises the intended routes.
- Save the configuration after confirming OSPF is active.

 

**26. Configure OSPF on the main campus router and cloud router** [01:06:55]

- Advertise all connected campus networks on the main router using OSPF.
- Use the correct wildcard masks for **/30** and **/24** networks.
- Configure the cloud router to advertise its connected networks as well.
- Run `show ip route ospf` to confirm learned routes.
- Verify that routing paths point through the correct next-hop interfaces.

 

**27. Validate end-to-end connectivity across the network** [01:09:07]

- From a client PC, test connectivity to devices outside the local subnet.
- Confirm that packets can traverse multiple routers and reach remote networks.
- Test access to the email server and other remote services.
- If all routes are correct, end-to-end communication should succeed.
- Document the final working state of the topology.

### Cautionary Notes

- **Do not enable CDP on end-device-facing ports** unless required; it can expose network details.
- **Match interface modes on both sides** of a link; mismatched access/trunk settings can cause connectivity issues.
- **Use /30 subnets for point-to-point router links** to conserve addresses and avoid overlap.
- **Keep static IPs outside DHCP pools** to prevent address conflicts.
- **Verify each step before moving on**; small mistakes in VLAN IDs, subinterface numbers, or wildcard masks can break routing.
- **Save configurations frequently** to avoid losing work during troubleshooting or device reloads.

### Tips for Efficiency

- Prepare commands in a text editor first, then paste them into devices to reduce typing errors.
- Use a consistent naming convention for VLANs, pools, and interfaces to simplify troubleshooting.
- Check `show vlan`, `show ip interface brief`, `show cdp neighbors`, and `show ip route ospf` after each major stage.
- Configure devices in a repeatable order: access switches first, then Layer 3 switches, then routers, then end devices.
- Watch terminal mismatch messages as a guide to identify unconfigured interfaces quickly.
- Document subnet-to-VLAN mappings in advance so DHCP pools and subinterfaces can be built faster.

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
