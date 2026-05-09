
# Redundant Enterprise Network Architecture

## 📌 Project Overview
This project demonstrates a production-ready branch office network. It focuses on high availability, logical segmentation, and secure remote management using Cisco IOS.

![Network Topology](topology/enterprise-network-topology.png)

## 🛠️ Key Features
*   **Logical Segmentation:** 3 VLANs (Sales, Guest, Management) implemented via Router-on-a-Stick (802.1Q).
*   **Redundancy:** Triangle topology between switches and router to eliminate single points of failure.
*   **Automated Services:** Integrated DHCP pools for dynamic IPv4 addressing.
*   **Security:** Hardened VTY lines with SSH v2 and RSA 2048-bit encryption.

## 🚀 How to Use
1. Download the `.pkt` (Packet Tracer) file from this repo.
2. Review the configurations in the `/configs` folder.
3. Verify connectivity using the proof-of-concept screenshots in `/docs`.

## ✅ Verification Commands
```bash
# To check routing logic:
show ip route
# To check VLAN trunking:
show interfaces trunk
