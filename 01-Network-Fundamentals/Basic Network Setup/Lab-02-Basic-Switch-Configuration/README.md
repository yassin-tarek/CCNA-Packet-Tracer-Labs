# Lab 02 - Basic Switch Configuration

## Objective

Perform the initial configuration of a Cisco switch by setting passwords, changing the hostname, configuring a login banner, and saving the configuration.

## Topology

<img width="845" height="482" alt="image" src="https://github.com/user-attachments/assets/680fab92-2545-48d6-8abc-ce6b68dfef00" />


## Devices Used

- 1 Cisco 2960 Switch
- 1 PC
- Console Connection

## Tasks Performed

- Changed the hostname
- Configured the enable secret password
- Configured the console password
- Configured the VTY password
- Enabled password encryption
- Configured a MOTD banner
- Saved the running configuration

## Commands Practiced

- hostname
- enable secret
- line console 0
- line vty 0 4
- login
- service password-encryption
- banner motd
- copy running-config startup-config

## Skills Practiced

- Basic switch configuration
- Cisco IOS CLI navigation
- Device security basics
- Saving configurations

## Files Included

- `Lab-02-Basic-Switch-Configuration.pkt`
- `topology.png`
- `README.md`

## Result

The switch was successfully configured with basic security settings and the configuration was saved to startup-config.
