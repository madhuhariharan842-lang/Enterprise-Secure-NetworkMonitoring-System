# Enterprise Secure Network Monitoring System

## Project Overview

This project demonstrates the design and implementation of an enterprise network infrastructure using Cisco Packet Tracer.

The network is segmented into multiple departments using VLANs and interconnected through Router-on-a-Stick inter-VLAN routing. Security controls such as DHCP and Extended ACLs have been implemented to simulate a real-world enterprise environment.

---

# Network Architecture

| Department | VLAN    | Network Address | Gateway      |
| ---------- | ------- | --------------- | ------------ |
| HR         | VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| IT         | VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
| Finance    | VLAN 30 | 192.168.30.0/24 | 192.168.30.1 |
| Guest      | VLAN 40 | 192.168.40.0/24 | 192.168.40.1 |

---

# Phase 1 - Enterprise Network Design

## Features Implemented

* VLAN Segmentation
* Inter-VLAN Routing (Router-on-a-Stick)
* Wireless Guest Network
* File Server Integration
* Network Printer Connectivity
* Connectivity Validation

---

## Network Topology

![Network Topology](TOPOLOGY.png)

---

## VLAN Verification

![VLAN Verification](VLAN-VERIFICATION.png)

---

## Connectivity Validation

![Connectivity Validation](CONNECTIVITY-VALIDATION.png)

---

# Phase 2 - DHCP and Security Implementation

## DHCP Configuration

The Cisco Router was configured as a DHCP Server to automatically assign IP addresses to all VLANs.

### DHCP Pools Created

* HR VLAN (10)
* IT VLAN (20)
* Finance VLAN (30)
* Guest VLAN (40)

### DHCP Benefits

* Automatic IP Address Assignment
* Centralized Network Management
* Reduced Configuration Errors

---

## Access Control Lists (ACLs)

Extended ACLs were implemented to isolate the Guest Network from internal enterprise resources.

### Security Policies

| Source               | Destination        | Action |
| -------------------- | ------------------ | ------ |
| Guest VLAN           | HR VLAN            | Deny   |
| Guest VLAN           | IT VLAN            | Deny   |
| Guest VLAN           | Finance VLAN       | Deny   |
| Guest VLAN           | File Server        | Deny   |
| Internal Departments | Internal Resources | Allow  |

---

## ACL Configuration

![ACL Configuration](ACL-CONFIGURATION.png)

---

## Security Validation

Guest devices were unable to access internal enterprise resources while authorized departmental communication remained operational.

![Security Validation](SECURITY-VALIDATION.png)

---

# Phase 3 - Security Monitoring and Attack Simulation

## Objective

Validate that implemented security controls prevent unauthorized access while maintaining normal business operations.

---

## Attack Simulation

Simulated unauthorized access attempts from the Guest VLAN to protected enterprise resources.

### Test Results

| Source               | Destination        | Result  |
| -------------------- | ------------------ | ------- |
| Guest VLAN           | HR VLAN            | Blocked |
| Guest VLAN           | IT VLAN            | Blocked |
| Guest VLAN           | Finance VLAN       | Blocked |
| Guest VLAN           | File Server        | Blocked |
| Internal Departments | Internal Resources | Allowed |

---

## Security Monitoring Summary

The implemented ACL policies successfully prevented unauthorized access attempts while maintaining communication between legitimate business departments.

### Security Events Observed

* Unauthorized Guest Access Attempt → Blocked
* Guest to File Server Access Attempt → Blocked
* Internal Department Communication → Allowed

---

## Conclusion

The Enterprise Secure Network Monitoring System successfully demonstrates:

* Enterprise VLAN Segmentation
* Router-on-a-Stick Inter-VLAN Routing
* DHCP Automation
* Extended ACL Security Controls
* Guest Network Isolation
* Security Monitoring
* Attack Simulation
* Security Validation

---

# Technologies Used

* Cisco Packet Tracer
* VLAN Configuration
* Inter-VLAN Routing
* Router-on-a-Stick
* DHCP
* Extended ACLs
* Network Security
* Switching and Routing

---

# Skills Demonstrated

* Enterprise Network Design
* VLAN Segmentation
* Inter-VLAN Routing
* DHCP Configuration
* Access Control Lists (ACLs)
* Security Monitoring
* Network Troubleshooting
* Security Validation
* Technical Documentation

---

# Future Enhancements

## Phase 4 - Enterprise Expansion

Planned enhancements:

* Multi-Branch Enterprise Network
* OSPF Dynamic Routing
* WAN Connectivity
* Branch Office Integration
* Advanced Network Monitoring

---

## Repository Contents

* Enterprise-Network-Design.pkt
* TOPOLOGY.png
* VLAN-VERIFICATION.png
* CONNECTIVITY-VALIDATION.png
* ACL-CONFIGURATION.png
* SECURITY-VALIDATION.png
* README.md

---

### Author

Madhu Hariharan

Enterprise Networking & Cybersecurity Learning Project

