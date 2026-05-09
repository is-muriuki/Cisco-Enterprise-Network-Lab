# 🏢 Cisco Enterprise Network Lab
[![Cisco IOS](https://img.shields.io/badge/Cisco-IOS-blue?logo=cisco)](https://www.cisco.com)
[![Topology](https://img.shields.io/badge/Topology-Layer%202%2F3-green)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> A production-ready branch office network simulating real enterprise environments using Cisco Packet Tracer. Covers Router-on-a-Stick, VLAN segmentation, OSPF routing, and secure remote management.

---

## 📌 Project Overview

This lab demonstrates a scalable Layer 2/3 network architecture suitable for a branch office environment. It is designed to simulate production-grade configurations with redundancy and logical segmentation.

**Key Technologies:**
- Router-on-a-Stick (inter-VLAN routing)
- VLAN segmentation (Sales, IT, Management)
- OSPF dynamic routing
- SSH remote management
- STP/RSTP for loop prevention

---

## 🗂️ Repository Structure

```
Cisco-Enterprise-Network-Lab/
├── Topology/          # Packet Tracer (.pkt) files
├── configs/           # Device configuration files
│   ├── router.txt
│   ├── core-switch.txt
│   └── access-switch.txt
└── README.md
```

---

## 🖧 Network Topology

![Network Topology](https://github.com/is-muriuki/Cisco-Enterprise-Network-Lab/commit/b2ad06ed45711f096ccafc4fb590e3ac1612e46d#diff-5dd17f23599fbea4e05058809e538dabf9eca45e142b2893375d734820e6177e)

| Device       | Role              | IP Address       |
|-------------|-------------------|-----------------|
| Router1    | Gateway / RoaS    | 192.168.1.1     |
| Core-SW      | Layer 3 Switch    | 192.168.1.2     |
| Access-SW1   | Access Layer      | 192.168.10.1    |

---

## 🔧 VLAN Design

| VLAN ID | Name       | Subnet           | Purpose              |
|---------|------------|-----------------|----------------------|
| 10      | Sales      | 192.168.10.0/24 | End user devices     |
| 20      | IT         | 192.168.20.0/24 | Server & admin hosts |
| 99      | Management | 192.168.99.0/24 | Device management    |

---

## 🚀 Getting Started

### Prerequisites
- Cisco Packet Tracer 8.x or later
- Basic understanding of Cisco IOS CLI

### Steps
1. Clone the repository
   ```bash
   git clone https://github.com/is-muriuki/Cisco-Enterprise-Network-Lab.git
   ```
2. Open `Topology/` folder in Cisco Packet Tracer
3. Review device configs in `configs/`
4. Use `show` commands to verify connectivity

---

## ✅ Features Implemented

- [x] VLAN creation and trunking
- [x] Router-on-a-Stick configuration
- [x] OSPF routing between segments
- [x] SSH access with local authentication
- [ ] DHCP server configuration (planned)
- [ ] ACL security policies (planned)

---

## 📚 Skills Demonstrated

`Cisco IOS` `VLAN` `OSPF` `STP` `Router-on-a-Stick` `Network Security` `Subnetting`

---

## 📄 License
MIT — feel free to use and adapt for learning purposes.

