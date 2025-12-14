🏥 Hospital Network Management System (Cisco Packet Tracer)
<div align="center"> <img src="hospital logo.png" alt="Hospital Network Logo" width="300"> </div>

A simulated hospital network infrastructure implemented using Cisco Packet Tracer. This project demonstrates hierarchical network design, inter-VLAN communication, routing, security, and VPN connectivity between Headquarters (HQ) and a Branch Office.

📑 Table of Contents

🚀 Features

🛠 Technologies & Tools

📁 Project Structure

🌐 Network Architecture

🗺️ Implementation Steps

🔒 Security Features

📄 Documentation

👥 Team Members

🚀 Features

Hierarchical Network Design: Core routers, multilayer switches, and access switches for HQ and Branch.

VLAN & Subnet Management: Each department in a separate VLAN with correct subnetting for 60 users (HQ) and 30 users (Branch).

Dynamic & Static IP Addressing: DHCP for user devices and static IPs for servers.

Inter-VLAN Routing: Multilayer switches provide inter-VLAN communication.

Routing Protocols: OSPF for dynamic routing and static default routes.

Internet Connectivity: Dual ISP configuration with public IPs.

Security Features: SSH remote login, port security with sticky MAC, and violation shutdown mode.

VPN & NAT: Site-to-site IPSec VPN and PAT for secure communication and Internet access.

Wireless Connectivity: Departmental wireless networks for staff and devices.

🛠 Technologies & Tools
Category	Technology / Tool	Purpose
Simulation	Cisco Packet Tracer	Network design & simulation
Routing	OSPF, Static Routes	Routing & connectivity management
Security	SSH, Port Security, ACLs	Secure remote access & access control
NAT & VPN	PAT, IPSec VPN	Internet access & secure branch connectivity
📁 Project Structure
Hospital_Network/
├── HospitalNetwork.pkt       # Cisco Packet Tracer project file
├── Image/                    # Network diagrams & topology screenshots
│   ├── hospital_network.png
│   ├── vlan_setup.png
│   └── topology.png
├── README.md                 # Project overview & documentation

🌐 Network Architecture

Headquarters (HQ):

Core Router

2 Multilayer Switches

Access Switches for Departments

Servers (DHCP, Database, File, etc.)

Departmental Wireless Networks

Branch Office:

Core Router

Multilayer Switches

Access Switches

Departmental Wireless Networks

Connectivity:

Serial connection between HQ and Branch

Internet via dual ISP with static IPs

Inter-VLAN routing for department communication

Site-to-site VPN for secure HQ-Branch communication

🗺️ Implementation Steps

Physical Design:

Place routers, switches, and hosts in HQ & Branch.

Connect devices according to hierarchical model.

IP Addressing & VLANs:

Subnet the network for all departments.

Assign VLANs for each department.

DHCP for user devices, static IP for servers.

Routing Configuration:

Configure OSPF on routers and multilayer switches.

Set static default routes for unknown traffic.

Inter-VLAN Communication:

Configure Router-on-a-Stick or multilayer switch routing.

Ensure devices from different VLANs can communicate.

Security Setup:

Enable SSH on all routers and switches.

Configure port security (sticky MAC, violation shutdown) for servers.

Apply ACLs for network access control.

VPN & NAT:

Configure site-to-site IPSec VPN between HQ and Branch.

Set up PAT for outbound internet access.

Wireless Network:

Deploy Wi-Fi in each department for device connectivity.

🔒 Security Features

SSH for secure remote administration.

Port security to limit unauthorized devices.

ACLs for traffic filtering.

Site-to-site VPN for encrypted branch communication.

NAT/PAT for secure internet access from private network.

📄 Documentation

hospital_network.png – Full network topology diagram

vlan_setup.png – VLAN and subnetting setup

topology.png – Detailed device connections and IP assignments

(Screenshots captured from Cisco Packet Tracer simulation.)

👥 Team Members
Name	
Umme Nafisa Anzum Kotha	Student 
Muttakin Mahmud	Teacher / Section Officer
💡 Notes

This project does not run as software. It is a network simulation in Cisco Packet Tracer.

The .pkt file contains the full configured network and can be opened in Cisco Packet Tracer for testing.
