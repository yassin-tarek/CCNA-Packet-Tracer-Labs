# Lab 04 - Connecting Two LANs with a Router

## Objective

Connect two different Local Area Networks (LANs) using a router and verify communication between devices on different networks.

## Topology

<img width="1103" height="477" alt="topology" src="https://github.com/user-attachments/assets/6ed252ae-7894-4e63-94a5-ed1b071d3626" />


## Devices Used

- 1 Cisco Router (1941/2911)
- 2 Cisco 2960 Switches
- 2 PCs
- Copper Straight-Through Cables

## IP Addressing

| Device | Interface | IP Address | Subnet Mask | Default Gateway |
|---------|-----------|------------|-------------|-----------------|
| PC0 | NIC | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| R1 | GigabitEthernet0/1 | 192.168.1.1 | 255.255.255.0 | - |
| R1 | GigabitEthernet0/0 | 192.168.2.1 | 255.255.255.0 | - |
| PC1 | NIC | 192.168.2.10 | 255.255.255.0 | 192.168.2.1 |

## Configuration

### Router Configuration

```bash
enable
configure terminal

hostname R1

interface g0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit

interface g0/1
ip address 192.168.2.1 255.255.255.0
no shutdown
exit

end

copy running-config startup-config
```

## Configuration Steps

1. Connect each PC to its switch.
2. Connect each switch to the router.
3. Configure the router interfaces.
4. Assign IPv4 addresses to both PCs.
5. Configure the correct default gateway on each PC.
6. Verify connectivity using the `ping` command.

## Verification

- Ping from **PC0** to **PC1**
- Ping from **PC1** to **PC0**
- Verify that both pings are successful.

## Skills Practiced

- Router configuration
- Interface configuration
- IPv4 addressing
- Default gateway configuration
- Inter-network communication
- Connectivity verification

## Files Included

- `Lab-04-Connecting-Two-LANs-with-a-Router.pkt`
- `topology.png`
- `README.md`

## Result

Both LANs successfully communicate through the router, demonstrating basic Layer 3 routing and the importance of the default gateway.
