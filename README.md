 Enterprise-Secure-NetworkMonitoring-System
 Enterprise Secure Network Monitoring System

 Project Overview

This project demonstrates the design and implementation of an enterprise network infrastructure using Cisco Packet Tracer.

The network is segmented into multiple departments using VLANs and interconnected through Router-on-a-Stick inter-VLAN routing.

---

 Network Architecture
 Departments

| Department | VLAN    | Network Address | Gateway      |
| ---------- | ------- | --------------- | ------------ |
| IT         | VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| HR         | VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
| Finance    | VLAN 30 | 192.168.30.0/24 | 192.168.30.1 |
| Guest      | VLAN 40 | 192.168.40.0/24 | 192.168.40.1 |

---

 Features Implemented

* VLAN Segmentation
* Inter-VLAN Routing (Router-on-a-Stick)
* Wireless Guest Network
* File Server Integration
* Network Printer Connectivity
* Static IP Addressing
* Connectivity Validation using ICMP
* Enterprise Network Design


 Devices Used

* Cisco 2911 Router
* Cisco 2960 Switch
* File Server
* Network Printer
* Access Point
* Desktop PCs
* Laptop
* Smartphone



 Validation Performed

Successful communication was verified between:

* IT ↔ HR
* Finance ↔ IT
* IT ↔ Guest Network
* File Server ↔ IT

This confirms proper VLAN configuration and inter-VLAN routing functionality.



 Technologies Used

* Cisco Packet Tracer
* VLAN Configuration
* Router-on-a-Stick
* Switching
* Routing
* IP Addressing
* Network Troubleshooting


 Skills Demonstrated

* Enterprise Network Design
* Network Segmentation
* VLAN Implementation
* Inter-VLAN Routing
* Wireless Network Configuration
* Connectivity Testing
* Network Documentation



 Future Enhancements

Phase 2 will include:

* Access Control Lists (ACLs)
* Security Policy Enforcement
* Simulated Attack Detection
* Security Monitoring
* Firewall-Based Restrictions
