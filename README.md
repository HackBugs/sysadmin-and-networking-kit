# 🛠️ sysadmin-kit

 > A practical collection of tools, software, labs, and resources for **System Administration, Networking, CCTV & IT Infrastructure**.

---

 ## 📊 Dashboard

 | Category | Tool / Resource | Status | Purpose |
| --- | --- | --- | --- |
| 🌐 Networking | **Cisco Packet Tracer** | 🟢 Free | Network simulation & labs |
| 🔬 Network Analysis | **Wireshark** | 🟢 Free | Packet capture & troubleshooting |
| 🖥️ Advanced Networking | **GNS3** | 🟢 Free | Advanced network simulation |
| 📹 CCTV | **IP Camera / VMS Labs** | 🟡 Lab | CCTV networking & configuration |

---

 # Download Cisco Packet Tracer and 🌐 Networking Lab

 ## Cisco Packet Tracer

 **Cisco Packet Tracer** is a network simulation tool that allows you to practice networking concepts without physical networking equipment.

 ### 🔐 Login

 Visit Cisco Networking Academy:

 **https://www.netacad.com/**  
 - [Download - Cisco Packet Tracer](https://skillsforall.com/resources/lab-downloads)

 ### 📚 Find Packet Tracer

 After logging in:

```
Search
  ↓
Getting Started with Cisco Packet Tracer
  ↓
Cisco Packet Tracer Resources
  ↓
Download Cisco Packet Tracer
```

 ### 💻 Downloads

 | Platform | Version | Architecture |
| --- | --- | --- |
| 🍎 macOS | `8.2.2` | 64-bit |
| 🐧 Ubuntu | `8.2.2` | 64-bit |
| 🪟 Windows | `8.2.2` | 64-bit |

> **Note:** Download the installer that matches your operating system.

---

 ## 🧪 What to Practice

 ### Beginner

 - [ ] Basic network topology
- [ ] PC ↔ Switch connection
- [ ] IP addressing
- [ ] Subnetting
- [ ] Ping testing
- [ ] MAC address table
- [ ] Basic switch configuration

 ### Intermediate

 - [ ] Router configuration
- [ ] DHCP
- [ ] VLAN
- [ ] Trunking
- [ ] Inter-VLAN routing
- [ ] Static routing
- [ ] DNS concepts

 ### CCTV Networking

 - [ ] IP Camera network design
- [ ] Camera IP addressing
- [ ] PoE switch concept
- [ ] NVR network architecture
- [ ] Camera ↔ Switch ↔ NVR topology
- [ ] Remote access concepts
- [ ] Network troubleshooting

---

 # 🔬 Network Analysis

 ## Wireshark

 Use Wireshark to inspect and troubleshoot network traffic.

 ### Practice

 - [ ] ARP
- [ ] DHCP
- [ ] DNS
- [ ] TCP
- [ ] UDP
- [ ] ICMP
- [ ] HTTP
- [ ] RTSP concepts

 🔗 **Official:** https://www.wireshark.org/

---

 # 🖥️ Advanced Networking

 ## GNS3

 GNS3 is useful for more advanced and realistic network labs.

 ### Practice

 - [ ] Router labs
- [ ] Switching
- [ ] Routing protocols
- [ ] VLANs
- [ ] Network troubleshooting
- [ ] Multi-router topology

 🔗 **Official:** https://www.gns3.com/

---

 # 📹 CCTV Lab

 ### Virtual CCTV Learning Path

```
              ┌──────────────┐
              │  IP Camera   │
              └──────┬───────┘
                     │
                     ▼
              ┌──────────────┐
              │  PoE Switch  │
              └──────┬───────┘
                     │
              ┌──────┴───────┐
              ▼              ▼
        ┌──────────┐    ┌──────────┐
        │   NVR    │    │   PC     │
        └──────────┘    └──────────┘
```

 ### CCTV Topics

 | Topic | Lab |
| --- | --- |
| IP Addressing | ⬜ |
| Camera Networking | ⬜ |
| PoE Concept | ⬜ |
| NVR Networking | ⬜ |
| VLAN for CCTV | ⬜ |
| DHCP | ⬜ |
| Static IP | ⬜ |
| RTSP | ⬜ |
| ONVIF | ⬜ |
| Troubleshooting | ⬜ |

---

 # 🧰 Recommended Learning Path

```
                    sysadmin-kit
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
     Networking       CCTV           Analysis
          │              │              │
          ▼              ▼              ▼
 Packet Tracer      IP Camera       Wireshark
          │              │
          ▼              ▼
        GNS3           NVR/VMS
```

 ### 🚀 Suggested Order

 1. **Cisco Packet Tracer** — Networking fundamentals
2. **Wireshark** — Packet analysis & troubleshooting
3. **CCTV Networking** — IP camera, NVR, PoE concepts
4. **GNS3** — Advanced networking labs

---

 ## 📁 Repository Structure

```
sysadmin-kit/
│
├── networking/
│   ├── packet-tracer/
│   ├── gns3/
│   └── wireshark/
│
├── cctv/
│   ├── ip-camera/
│   ├── nvr/
│   ├── poe/
│   └── troubleshooting/
│
├── labs/
│   ├── beginner/
│   ├── intermediate/
│   └── advanced/
│
└── README.md
```

---

 ## 🎯 Goal

 > Build a complete **software-based IT lab** for learning Networking, System Administration, CCTV Networking, and Troubleshooting without requiring physical hardware at the beginning.

---

 ### 📌 Status Legend

 - 🟢 **Free**
- 🟡 **Lab / Learning**
- 🔵 **Recommended**
- ⬜ **Pending**
- ✅ **Completed**
