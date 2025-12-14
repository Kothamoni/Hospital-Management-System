# 🏥 Hospital Network Management System (Cisco Packet Tracer)

<div align="center">
  <img src="Image/hospital_network.png" alt="Hospital Network Logo" width="300">
</div>

<p align="center">
  <a href="https://www.cisco.com/">
    <img src="https://img.shields.io/badge/Cisco-Packet%20Tracer-1572B6?style=for-the-badge&logo=cisco&logoColor=white" alt="Cisco Packet Tracer Badge"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Network-Design-green?style=for-the-badge&logo=network-manager&logoColor=white" alt="Network Design Badge"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/VLAN-Subnet-blue?style=for-the-badge&logo=virtualbox&logoColor=white" alt="VLAN Badge"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Security-SSH-red?style=for-the-badge&logo=lock&logoColor=white" alt="Security Badge"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/VPN-NAT-orange?style=for-the-badge&logo=vpn&logoColor=white" alt="VPN Badge"/>
  </a>
</p>

A simulated **hospital network infrastructure** implemented using **Cisco Packet Tracer**. This project demonstrates hierarchical network design, inter-VLAN communication, routing, security, and VPN connectivity between **Headquarters (HQ)** and a **Branch Office**.

---

## 📑 Table of Contents
- 🚀 [Features](#-features)  
- 🛠 [Technologies & Tools](#-technologies--tools)  
- 📁 [Project Structure](#-project-structure)  
- 🌐 [Network Architecture](#-network-architecture)  
- 🗺️ [Implementation Steps](#-implementation-steps)  
- 🔒 [Security Features](#-security-features)  
- 📄 [Documentation](#-documentation)  
- 👥 [Team Members](#-team-members)  

---

## 🚀 Features
- **Hierarchical Network Design:** Core routers, multilayer switches, and access switches for HQ and Branch.  
- **VLAN & Subnet Management:** Separate VLAN for each department; subnetting for 60 users (HQ) and 30 users (Branch).  
- **Dynamic & Static IP Addressing:** DHCP for devices, static IPs for servers.  
- **Inter-VLAN Routing:** Communication across VLANs via multilayer switches.  
- **Routing Protocols:** OSPF for dynamic routing, static default routes.  
- **Internet Connectivity:** Dual ISP with public IPs.  
- **Security Features:** SSH remote login, port security with sticky MAC, violation shutdown mode.  
- **VPN & NAT:** Site-to-site IPSec VPN and PAT for secure communication.  
- **Wireless Connectivity:** Departmental Wi-Fi networks.  

---

## 🛠 Technologies & Tools

| Category         | Technology / Tool          | Purpose                                |
|-----------------|---------------------------|----------------------------------------|
| Simulation       | Cisco Packet Tracer       | Network design & simulation            |
| Routing          | OSPF, Static Routes       | Routing & connectivity management      |
| Security         | SSH, Port Security, ACLs  | Secure remote access & access control  |
| NAT & VPN        | PAT, IPSec VPN            | Internet access & secure branch connectivity |

---
📂 Project Structure
Hospital_Network/
├── .gitignore               # Excludes temporary and unnecessary files
├── HospitalNetwork.pkt      # The main Cisco Packet Tracer configuration file
├── Image/                   # Network diagrams & screenshots
│   ├── hospital_network.png   # High-level logical or physical diagram
│   ├── vlan_setup.png         # Screenshot/diagram of VLAN & Inter-VLAN config
│   └── topology.png           # General network topology or subnet map
├── README.md                # Project overview, requirements, and implementation steps
└── requirements.md          # Dedicated file for the detailed requirements (Optional, but good practice)

## 🌐 Network Architecture

**Headquarters (HQ):**
- Core Router  
- 2 Multilayer Switches  
- Access Switches for Departments  
- Servers (DHCP, Database, File, etc.)  
- Departmental Wireless Networks  

**Branch Office:**
- Core Router  
- Multilayer Switches  
- Access Switches  
- Departmental Wireless Networks  

**Connectivity:**
- Serial connection between HQ and Branch  
- Internet via dual ISP with static IPs  
- Inter-VLAN routing for department communication  
- Site-to-site VPN for secure HQ-Branch communication  

---

## 🗺️ Implementation Steps

1. **Physical Design:** Place routers, switches, and hosts in HQ & Branch. Connect devices according to hierarchical model.  
2. **IP Addressing & VLANs:** Subnet network, assign VLANs, configure DHCP & static IPs.  
3. **Routing Configuration:** Configure OSPF on routers and multilayer switches. Set static default routes.  
4. **Inter-VLAN Communication:** Enable Router-on-a-Stick or multilayer switch routing.  
5. **Security Setup:** Enable SSH, configure port security & ACLs.  
6. **VPN & NAT:** Configure site-to-site IPSec VPN and PAT.  
7. **Wireless Network:** Deploy Wi-Fi for all departments.  

---

## 🔒 Security Features

- SSH for secure remote administration  
- Port security to limit unauthorized devices  
- ACLs for traffic filtering  
- Site-to-site VPN for encrypted communication  
- NAT/PAT for secure internet access  

---

## 📄 Documentation

- `hospital_network.png` – Full network topology diagram  
- `vlan_setup.png` – VLAN & subnet configuration  
- `topology.png` – Device connections & IP assignments  

*(Screenshots captured from Cisco Packet Tracer simulation.)*

---

## 👥 Team Members

| Name                     |                             
|--------------------------|
| Umme Nafisa Anzum Kotha  |  
| Muttakin Mahmud          |

---

💡 **Notes:**  
This project **does not run as software**. It is a **network simulation** in Cisco Packet Tracer. The `.pkt` file contains the full configured network and can be opened for testing.

---

