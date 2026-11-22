# Enterprise Network Design: Switching, Routing & Layer 2 Security

Design and simulation of a two-site enterprise network (Kuala Lumpur HQ with server farm, and a Krung Thep branch) in Cisco Packet Tracer: VLAN segmentation, dynamic routing, redundancy, wireless and Layer 2 attack mitigation.

**Full write-up:** [writeup.md](writeup.md) · **Simulation:** [`packet-tracer/enterprise-network.pkt`](packet-tracer/enterprise-network.pkt) (Cisco Packet Tracer 8.x)

## What Was Built

**Switching & routing**
- Network diagrams and an IPv4 addressing plan (private LANs, server farm, WAN public addressing)
- **VLANs and 802.1Q trunking** per department (Design, Delivery, HR …)
- **Inter-VLAN routing** (router-on-a-stick) at both sites
- **OSPF** dynamic routing between sites
- **Spanning Tree Protocol** configuration
- **EtherChannel** link aggregation for bandwidth and redundancy
- **HSRP** first-hop redundancy (verified with traceroute)
- **DHCP** services for the branch network

**Wireless**
- WLAN architecture with a **Wireless LAN Controller (WLC)**: pre-setup, virtual interfaces, WLAN creation and AP groups

**Server farm**
- DNS, web and FTP servers, with connectivity testing (ping/tracert matrix)

**Layer 2 security**
- Threat analysis: MAC address table flooding, VLAN hopping, DHCP starvation, ARP spoofing/poisoning, STP attacks
- Mitigations: **port security**, VLAN hopping protection (native VLAN / trunk hardening), **BPDU Guard / PortFast**, **DHCP snooping**, and ACLs

## Tools & Concepts

Cisco Packet Tracer · VLAN · 802.1Q · Inter-VLAN routing · OSPF · STP · EtherChannel · HSRP · DHCP · WLC · ACLs · Port security · DHCP snooping · BPDU Guard

Team project.
