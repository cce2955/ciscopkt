# Cisco Packet Tracer Network Project

## Overview

This project demonstrates a complex network topology set up using Cisco Packet Tracer. It showcases advanced networking skills, including routing, switching, DHCP configuration, and access control.

## Topology

```plaintext
SW1       SW2
|         |
R1 ------ R2
|
R4 ------ R3
|         |
SW4       SW3
```



## Technologies Used

1. **Routing**: OSPF (Open Shortest Path First) is used for dynamic routing between routers to ensure effective inter-router communication.
2. **DHCP**: Dynamic Host Configuration Protocol is set up on routers to dynamically assign IP addresses to End User devices.
3. **Access Control**: Access Control Lists (ACLs) are implemented to control traffic flow between specific routers, demonstrating a proficiency in network security measures. To be more clear, the end user devices on R4 are block from communicating with the devices on R2, while still having communication with other routers

## Purpose

The main purpose of this project is to:

1. Exhibit a mastery of setting up and configuring a multi-router and multi-switch environment.
2. Showcase the ability to design and implement complex IP addressing schemes.
3. Demonstrate proficiency in setting up DHCP for automatic IP assignment.
4. Display skills in implementing OSPF as a dynamic routing protocol.
5. Highlight advanced access control techniques using ACLs.

## Key Features

1. **Segmented Network**: The network is divided into multiple segments, each with its own IP range, providing an organized and scalable design.
2. **Robust Routing**: OSPF ensures that all routers are aware of all routes in the network, providing redundancy and efficient path selection.
3. **Dynamic IP Assignment**: End-user devices receive their IP addresses from a DHCP pool, simplifying network management.
4. **Selective Communication**: Using ACLs, selective communication is enforced, such as restricting communication between R4 and R2.

## Conclusion

This Packet Tracer project is a testament to advanced networking skills and the ability to design, implement, and manage complex network topologies. It serves as an excellent reference for anyone looking to understand advanced networking concepts in a practical setting.

