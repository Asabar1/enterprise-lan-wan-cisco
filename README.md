# Enterprise LAN/WAN Network Design & Implementation

A multi-site enterprise network simulation built in **Cisco Packet Tracer**, demonstrating end-to-end network design including subnetting, VLAN segmentation, inter-VLAN routing, DMZ architecture, and WAN connectivity.

## 📋 Project Overview

This project simulates a real-world enterprise network for multiple companies located in different cities, interconnected through a Wide Area Network (WAN). The design covers everything from IP address planning to security architecture.

**Scale:** 230+ users across 7 subnets per company site

## 🛠️ Skills Demonstrated

- **Subnetting:** VLSM (Variable-Length Subnet Masking) and CIDR
- **LAN Design:** VLANs, router subinterfaces, inter-VLAN routing, trunk links
- **WAN Design:** Static routing across multiple sites
- **Network Security:** DMZ architecture isolating public-facing services
- **Network Services:** DHCP, DNS, FTP, Web, and Email server integration
- **Wireless:** Guest WLAN with isolated subnet
- **Routing Protocol Analysis:** Comparison of Static, RIPv2, and OSPFv2
- **Verification:** End-to-end connectivity testing with ping/ICMP

## 🏗️ Network Architecture

### Per-Site LAN Design
- **Engineering** — VLAN 10
- **Manufacturing** — VLAN 20
- **Sales/Marketing** — VLAN 30
- **Administration** — VLAN 40
- **Internal Servers** — VLAN 50 (DHCP, DNS, FTP)
- **DMZ** — Web & Email servers (isolated from internal LAN)
- **Guest WLAN** — VLAN 70 (visitor access, restricted to web servers only)

### WAN Design
- Central WAN router (R-WAN) interconnecting company sites
- Static routing for predictable, low-overhead path selection
- /30 point-to-point links between each company router and R-WAN

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `SABAR_LAN_WAN_Project.pkt` | Cisco Packet Tracer simulation file |
| `407 progress report#1.pdf` | IP addressing & VLSM subnet allocation |
| `progress report #2.pdf` | LAN topology design and configuration |
| `Progress report #3.pdf` | WAN implementation and routing |
| `ECE 407 final report (2).pdf` | Complete project documentation |

## ▶️ How to View the Simulation

1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (free)
2. Open `Sabar_LAN_WAN_Project.pkt`
3. Use the CLI on any router to inspect configurations:
   - `show running-config`
   - `show ip route`
   - `show ip interface brief`
4. Test connectivity by pinging between devices in different subnets

## 📝 Notes

The progress reports document the original design including a third company site. The included Packet Tracer file demonstrates a fully working multi-site WAN implementation.

## 👤 Author

**Abdul Rahim Sabar**
Computer and Cybersecurity Engineering Student — Illinois Institute of Technology
