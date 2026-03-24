Enterprise Network Design with WAN Connectivity

**Overview**

This project demonstrates the design and implementation of a multi-site enterprise network using Cisco Packet Tracer. The network consists of multiple Local Area Networks (LANs) interconnected through a Wide Area Network (WAN) using routers.

The objective of this lab is to simulate real-world enterprise networking by configuring routing, IP addressing, and ensuring end-to-end connectivity between different subnets.

**Network Architecture**

The topology consists of:

=> **4 LANs (Departments / Locations):**
  - LAN 1: 192.168.1.0/24
  - LAN 2: 192.168.2.0/24
  - LAN 3: 192.168.3.0/24
  - LAN 4: 192.168.4.0/24
 
=> **4 Routers and their addresses**

  - Router 1 - 2: 10.0.12.1 - 10.0.12.2
  - Router 3 - 1: 10.0.25.1 - 10.0.25.2
  - Router 3 - 4: 10.0.34.1 - 10.0.34.2
  - Router 4 - 2: 10.0.23.1 - 10.0.23.2

=> Routers connected in a WAN topology (multi-hop communication)

=> Switches connecting end-user devices (PCs)

=> End Devices: Multiple hosts in each subnet

=> Network Topology

![Network Topology](topology/network-topology.png)
https://github.com/Ayomide101-debug/Cisco-WAN-lab/blob/main/Enterprise%20WAN%20Image.png?raw=true

Key Features & Configurations

=> **IP Addressing**
- Each LAN is assigned a /24 subnet
- Default gateways configured on routers
- Logical segmentation of networks for scalability

=> **Routing**
- Static routing implemented across routers
- Routes configured to enable full communication between all subnets
  
=> *Interfaces*
- **GigabitEthernet (G0/x):** Used for inter-router WAN links  
- **FastEthernet (Fa0/x):** Used for LAN connections  

=> **Testing & Verification**

Connectivity across the network was verified using:

- 'ping' tests between hosts in different subnets  
- Successful packet transmission across multiple routers  
- Validation of routing tables using:
  **show ip route**
