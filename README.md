# Multi-Router Network Configuration

This project establishes a network topology involving four routers. Each router serves its own local network, and they are interconnected to facilitate communication between different end-user devices.

## Network Topology

- **Router1 (R1)**:
  - Local Network: 192.168.1.x
  - Interface: GigabitEthernet0/1
    - IP: 10.0.0.1/30

- **Router2 (R2)**:
  - Local Network: 192.168.2.x
  - Interface: GigabitEthernet0/1
    - IP: 10.0.0.2/30
  - Interface: GigabitEthernet0/2
    - IP: 10.0.1.2/30

- **Router3 (R3)**:
  - Local Network: 192.168.3.x
  - Interface: GigabitEthernet0/1
    - IP: 10.0.1.1/30
  - Interface: GigabitEthernet0/2
    - IP: 10.0.2.1/30

- **Router4 (R4)**:
  - Local Network: 192.168.4.x
  - Interface: GigabitEthernet0/1
    - IP: 10.0.2.2/30

## Communication Flow

1. **R1** communicates with **R2** via the 10.0.0.0/30 network.
2. **R2** communicates with **R3** via the 10.0.1.0/30 network.
3. **R3** communicates with **R4** via the 10.0.2.0/30 network.
4. All Routers are able to communicate directly wth each other
## Project Objectives

- Ensure all end-user devices can communicate across routers.
- Configure static routes to manage inter-router communication.
- Maintain network security by controlling inter-router communication paths.

## Usage

1. Set up the routers as per the given topology.
2. Configure interfaces with the provided IP addresses.
3. Assign IPs to end-user devices within their respective 192.168.x.0/24 networks.
4. Set up static routes on each router to ensure inter-router communication.
5. Test communication between end-user devices.

## Notes

- Make sure to regularly save your router configurations to avoid data loss.
- Monitor router interfaces to ensure they're up and operational.
- Adjust the network topology as needed based on project requirements.

## Conclusion

This project provides a foundational setup for a multi-router network environment. Each router serves its distinct local network, allowing devices to communicate within and across these networks.
