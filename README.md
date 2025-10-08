# CMPG325 Networks Individual Project-2025
Network Topologies Design &amp; Simulation, Feature Configuration using Cisco Packet Tracer.

**Name:** Tsholofelo Modisapudi 
**Student Number:** 38391716

---

## Table of Contents

### 1.0 Project Overview
- 1.1 Project Objectives

### 2.0 Phase I: Network Topologies Design & Simulation
- 2.1 Overall IP Addressing Plan (IPv4 & IPv6)
- 2.2 Individual Topology Documentation
  - 2.2.1 Bus Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence (Screenshots)
  - 2.2.2 Mesh Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence (Screenshots)
  - 2.2.3 Star Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence (Screenshots)
  - 2.2.4 Ring Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence (Screenshots)
  - 2.2.5 Extended Star Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence (Screenshots)

- 2.3 Hybrid Topology
  - 2.3.1 Design Concept and Rationale
  - 2.3.2 Final Hybrid Network Diagram
  - 2.3.3 Comprehensive IP Addressing Table
  - 2.3.4 VLAN Configuration
    - VLAN Table (ID, Name, Assigned Network)
    - Switch Configuration Screenshots
  - 2.3.5 Server Configuration (HTTP, DNS, DHCP)
    - Server IP Settings
    - Service Configuration Screenshots
  - 2.3.6 Hybrid Network Testing
    - Inter-VLAN Routing Test (Ping across segments)
    - HTTP Server Access Test (Web Browser)
    - DNS Resolution Test (Using Domain Name)
    - DHCP Functionality Test

### 3.0 Phase II: Individual Network Feature Configuration
- 3.1 WPA3 Security Implementation
  - 3.1.1 Wireless Access Point/Router Configuration
  - 3.1.2 WPA3 Security Settings Screenshot
  - 3.1.3 Wireless Client Connection Process
  - 3.1.4 Security and Integration Test (Ping from wireless client to wired network)

### 4.0 Phase III: Video Demonstration
- 4.1 Video Link
- 4.2 Video Outline and Summary

### 5.0 Project Reflection
- 5.1 Challenges Encountered
- 5.2 Key Learnings

### 6.0 Appendix
- 6.1 References
- 6.2 Packet Tracer Project Files (.pkt)

---

## Project Overview
### Project Objectives
CMPG 325 individual semester-long project Computer Networks aims to demonstrate comprehensive understanding of network design, implementation, and management through hands-on simulation using Cisco Packet Tracer. The primary objectives are:
- Design and implement five fundamental network topologies: Bus, Mesh, Star, Ring, and Extended Star
- Create and configure a hybrid topology that creatively integrates elements from multiple basic topologies
- Implement dual-stack networking with both IPv4 and IPv6 addressing schemes
- Configure network segmentation using VLAN technology
- Deploy and manage network services including HTTP web server, DNS, and DHCP
- Implement enterprise-grade wireless security using WPA3 protocol
- Document the entire process comprehensively on GitHub with proper version control
- Demonstrate functionality through a professional video presentation

---

## Bus Topology
### Design Schematic

[ PC2 ]                              [ PC0 ]
    |                                   |
    |                                   |
[ Switch11 ]-----[ Switch10 ]-----[ Switch9 ]-----[ Switch0 ]
(2950-24)         (2950T-24)      (2950T-24)       (2950T-24)
                    |                                   |
                    |                                   |
                [ Laptop0 ]                          [ PC1 ]

### IP Address Table
| Device Name | Model | IPv4 Address | Subnet Mask | Default Gateway |
|-------------|-------|--------------|-------------|----------------|
| PC0 | PC-PT | 192.168.1.3 | 255.255.255.0 | 192.168.1.1 |
| PC1 | PC-PT | 192.168.1.4 | 255.255.255.0 | 192.168.1.1 |
| PC21 | PC-PT | 192.168.1.6 | 255.255.255.0 | 192.168.1.1 |
| Laptop11 | Laptop-PT | 192.168.1.5 | 255.255.255.0 | 192.168.1.1 |


### Configuration Notes
Devices Used:
End Devices: 3x PC-PT, 1x Laptop-PT
Switches: 2950-24 Switch (x4)
Connections: Straight Through cables from end devices to switches. Cross Over cables between switches
Configuration Details:
IP Scheme: Manual static IP configuration
Subnet: Single flat network (192.168.1.0/24)
Gateway: 192.168.1.1

### Connectivity Test Evidence (Screenshots)
