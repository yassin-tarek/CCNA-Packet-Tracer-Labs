# Lab 01 - Two PCs Through a Switch

## Objective
Build a simple local area network (LAN) by connecting two PCs to a switch, assigning IPv4 addresses, and verifying connectivity using the `ping` command.

## Topology

<img width="1106" height="537" alt="image" src="https://github.com/user-attachments/assets/65412615-dca4-44be-a995-cf07adc3f798" />



## Devices Used

- 2 PCs
- 1 Cisco 2960 Switch
- Copper Straight-Through Cables

## IP Addressing

| Device | IP Address | Subnet Mask |
|--------|------------|-------------|
| PC0 | 192.168.1.10 | 255.255.255.0 |
| PC1 | 192.168.1.20 | 255.255.255.0 |

## Configuration Steps

1. Place one Cisco 2960 switch.
2. Add two PCs.
3. Connect each PC to the switch using Copper Straight-Through cables.
4. Configure the IPv4 address on each PC.
5. Save the Packet Tracer file.
6. Test connectivity using the `ping` command.

## Verification

- Ping from **PC0** to **PC1**
- Ping from **PC1** to **PC0**
- Both pings should be successful.

## Skills Practiced

- Basic network topology
- Connecting end devices
- IPv4 addressing
- LAN communication
- Connectivity testing with `ping`

## Files Included

- `Lab-01-Two-PCs-Through-a-Switch.pkt`
- `topology.png`
- `README.md`

## Result

Both PCs successfully communicate with each other through the switch, confirming correct network configuration.
