# Three-Router Network Setup in Cisco Packet Tracer

This document describes a network setup with three routers, each connected to its respective switch and end user device, with DHCP configured for local networks.

## Network Topology

- **Router1**
  - DHCP Pool for Local Network: `192.168.1.0/24`
  - Connected to **Router2** via `10.0.0.0/30`
- **Router2**
  - DHCP Pool for Local Network: `192.168.2.0/24`
  - Connected to **Router1** via `10.0.0.0/30`
  - Connected to **Router3** via `10.0.1.0/30`
- **Router3**
  - DHCP Pool for Local Network: `192.168.3.0/24`
  - Connected to **Router2** via `10.0.1.0/30`

## Configuration Steps

1. **Physical Setup**
   - Connect each router to its respective switch.
   - Connect an end user device (e.g., PC) to each switch.
   - Connect **Router1** to **Router2** (consider using a crossover cable).
   - Connect **Router2** to **Router3**.

2. **IP Address and DHCP Configuration**
   - Assign IPs to each router interface.
   - Set up DHCP on each router to provide IP addresses to end devices in their respective local networks.
     - Ensure the DHCP pool excludes the router's IP and any static IPs you've assigned.
     - Set the default gateway in the DHCP pool to the router's local IP.
   - Ensure end devices are set to obtain an IP address automatically.

3. **Routing**
   - Set up static routes to ensure each router knows about the other networks.
   - Ensure end-to-end connectivity between all devices.

## Testing

1. Check that end devices receive IP addresses from the DHCP pool.
2. Ping between end devices across different networks to ensure proper communication.
3. Use `show ip route` on routers to verify routing tables.
4. Use `show ip dhcp binding` on routers to see which devices have received IPs from DHCP.
5. Troubleshoot using ping between routers, checking interface statuses, and verifying IP configurations.

## Notes

- Ensure all interfaces are up (`no shutdown` command in Cisco devices).
- Double-check subnet masks and default gateways on end devices.
- For extended networks, consider using dynamic routing protocols like OSPF or EIGRP.

