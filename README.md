# Cisco Packet Tracer Network Simulation

## Overview

This Cisco Packet Tracer (.pkt) file simulates a network topology connecting 20 devices across two routers and two switches. The simulation showcases a basic network setup with interconnectivity between devices. This README provides an overview of the simulation and instructions for its use.

## Prerequisites

- Cisco Packet Tracer software (Version X.X or higher) installed on your computer.
- Basic understanding of networking concepts and Cisco Packet Tracer.

## Network Topology

The network topology consists of the following components:

- **Router1:** Cisco 2901 Series Router
  - GigabitEthernet0/0: Connected to Switch1
  - GigabitEthernet0/1: Connected to Router2

- **Router2:** Cisco 2901 Series Router
  - GigabitEthernet0/0: Connected to Switch2
  - GigabitEthernet0/1: Connected to Router1

- **Switch1:** Cisco 2960 Series Switch
  - FastEthernet0/1 to FastEthernet0/10: Connected to Devices 1-10
  - GigabitEthernet0/1: Connected to Router1

- **Switch2:** Cisco 2960 Series Switch
  - FastEthernet0/1 to FastEthernet0/10: Connected to Devices 11-20
  - GigabitEthernet0/1: Connected to Router2

- **Devices 1-20:** These represent end-user devices, such as PCs, laptops, or servers, connected to the switches.

## DHCP Pools

Each router provides DHCP services to a different subnet:

- **Router1 DHCP Pool (vlan1):**
  - Subnet: 192.168.2.0/24
  - Default Gateway: 192.168.2.1
  - DNS Server: 8.8.8.8

- **Router2 DHCP Pool (vlan2):**
  - Subnet: 192.168.3.0/24
  - Default Gateway: 192.168.3.1
  - DNS Server: 8.8.8.8

## Instructions

1. Open the simulation file using Cisco Packet Tracer.

2. To start the simulation, click on the "Play" button or navigate to the "Simulation" tab and choose "Realtime Mode."

3. Observe the network topology and the connectivity between devices, routers, and switches.

4. To interact with the devices, select a device, go to the "CLI" tab, and use the command-line interface to configure, troubleshoot, or ping other devices.

5. Experiment with various network configurations, IP addressing, and routing protocols to learn and practice networking concepts.

6. To stop the simulation, click on the "Stop" button or exit the "Realtime Mode."

## Additional Notes

- This simulation provides a basic network setup. Feel free to modify and expand the network as needed for your learning or testing purposes.

- Save your changes as a new Packet Tracer (.pkt) file if you want to preserve your configurations or experiments.

## Credits

This simulation was created for educational purposes and is not intended for production use.

## License

This Packet Tracer simulation is provided under the [MIT License](LICENSE).
