# Lab 03 - Three PCs on One LAN

## Objective

Configure three PCs connected to a switch and verify full connectivity within the same LAN.

## Topology

<img width="1176" height="590" alt="topology" src="https://github.com/user-attachments/assets/9df25ff7-9235-4099-ba8c-e31d1f4f91f5" />


## Devices Used

- 1 Cisco 2960 Switch
- 3 PCs
- Copper Straight-Through Cables

## IP Addressing

| Device | IP Address | Subnet Mask |
|---------|------------|-------------|
| PC0 | 192.168.1.10 | 255.255.255.0 |
| PC1 | 192.168.1.20 | 255.255.255.0 |
| PC2 | 192.168.1.30 | 255.255.255.0 |

## Configuration Steps

1. Connect all PCs to the switch.
2. Configure the IPv4 address on each PC.
3. Verify communication using the `ping` command.

## Verification

- PC0 can ping PC1 and PC2.
- PC1 can ping PC0 and PC2.
- PC2 can ping PC0 and PC1.

## Skills Practiced

- LAN setup
- IPv4 addressing
- Basic switch connectivity
- Network verification with `ping`

## Files Included

- `Lab-03-Three-PCs-One-LAN.pkt`
- `topology.png`
- `README.md`

## Result

All three PCs successfully communicate with each other on the same local area network.
