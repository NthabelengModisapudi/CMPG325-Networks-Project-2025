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
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence (Screenshots)
  - 2.2.2 Mesh Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence 
  - 2.2.3 Star Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence 
  - 2.2.4 Ring Topology
    - Design Schematic
    - IP Addressing Table
    - Configuration Notes
    - Connectivity Test Evidence 
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

## Network Topologies Design & Simulation

### Bus Topology
#### IP Address Table
| Device Name | Model | IPv4 Address | Subnet Mask | Default Gateway |
|-------------|-------|--------------|-------------|----------------|
| PC0 | PC-PT | 192.168.1.3 | 255.255.255.0 | 192.168.1.1 |
| PC1 | PC-PT | 192.168.1.4 | 255.255.255.0 | 192.168.1.1 |
| PC2 | PC-PT | 192.168.1.6 | 255.255.255.0 | 192.168.1.1 |
| Laptop0 | Laptop-PT | 192.168.1.5 | 255.255.255.0 | 192.168.1.1 |

#### Configuration Notes
Devices Used:
End Devices: 3x PC-PT, 1x Laptop-PT
Switches: 2950-24 Switch (x4)
Connections: Straight Through cables from end devices to switches. Cross Over cables between switches
Configuration Details:
IP Scheme: Manual static IP configuration
Subnet: Single flat network (192.168.1.0/24)
Gateway: 192.168.1.1

#### Connectivity Test Evidence (Screenshots)
<img width="1366" height="768" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/05c00b3f-a677-40d9-aeed-275871715ced" />

### Mesh Topology
#### IP Address Table
| Device Name | Model | IPv4 Address | Subnet Mask | Default Gateway |
|-------------|-------|--------------|-------------|----------------|
| PC21 | PC-PT | 192.168.4.3 | 255.255.255.0 | 192.168.4.1 |
| PC26 | PC-PT | 192.168.4.5 | 255.255.255.0 | 192.168.4.1 |
| PC27 | PC-PT | 192.168.4.6 | 255.255.255.0 | 192.168.4.1 |
| Laptop2 | Laptop-PT | 192.168.4.4 | 255.255.255.0 | 192.168.4.1 |

#### Configuration Notes
Devices Used:
End Devices: 3x PC-PT, 1x Laptop-PT
Switches: 2950-24 Switch (x4)
Connections: Straight Through cables from end devices to switches. Cross Over cables between switches
Configuration Details:
IP Scheme: Manual static IP configuration
Gateway: 192.168.4.1

#### Connectivity Test Evidence 
<img width="1366" height="768" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/04d41a53-b454-4ff3-85d6-55ec971d29e4" />

### Star Topology
#### IP Address Table
| Device Name | Model | IPv4 Address | Subnet Mask | Default Gateway |
|-------------|-------|--------------|-------------|----------------|
| PC6 | PC-PT | 192.168.3.7 | 255.255.255.0 | 192.168.3.1 |
| PC7 | PC-PT | 192.168.3.8 | 255.255.255.0 | 192.168.3.1 |
| PC8 | PC-PT | 192.168.3.6 | 255.255.255.0 | 192.168.3.1 |
| PC9 | PC-PT | 192.168.3.5 | 255.255.255.0 | 192.168.3.1 |
| Laptop1  | Laptop-PT | 192.168.3.4 | 255.255.255.0 | 192.168.3.1 |
| Laptop11 | Laptop-PT | 192.168.3.3 | 255.255.255.0 | 192.168.3.1 |

#### Configuration Notes
Devices Used:
End Devices: 4x PC-PT, 2x Laptop-PT
Switches: 2950T-24 Switch
Connections: Straight Through cables from end devices to one switch.
Configuration Details:
IP Scheme: Manual static IP configuration
Gateway: 192.168.3.1

#### Connectivity Test Evidence 
<img width="1366" height="768" alt="Screenshot (20)" src="https://github.com/user-attachments/assets/80d28d85-0f40-4949-8ba4-7ad9b15dc264" />

### Ring Topology
#### IP Address Table
| Device Name | Model | IPv4 Address | Subnet Mask | Default Gateway |
|-------------|-------|--------------|-------------|----------------|
| PC4  | PC-PT | 192.168.4.3 | 255.255.255.0 | 192.168.4.1 |
| PC5  | PC-PT | 192.168.4.4 | 255.255.255.0 | 192.168.4.1 |
| PC22 | PC-PT | 192.168.4.5 | 255.255.255.0 | 192.168.4.1 |
| PC23 | PC-PT | 192.168.4.7 | 255.255.255.0 | 192.168.4.1 |
| PC24 | PC-PT | 192.168.4.8 | 255.255.255.0 | 192.168.4.1 |
| PC25 | PC-PT | 192.168.4.6 | 255.255.255.0 | 192.168.4.1 |

#### Configuration Notes
Devices Used:
End Devices: 6x PC-PT
Switches: 2950-24 Switch (x5)
Connections: Straight Through cables from end devices to switches. Cross Over cables between switches
Configuration Details:
IP Scheme: Manual static IP configuration
Gateway: 192.168.4.1

#### Connectivity Test Evidence 
<img width="1366" height="768" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/47e90006-7a0e-4f35-9f83-a6c745a21851" />

### Extended Star Topology
#### Design Schematic
#### IP Address Table
| Device Name | Model | IPv4 Address | Subnet Mask | Default Gateway |
|-------------|-------|--------------|-------------|----------------|
| PC20 | PC-PT | 192.168.2.23 | 255.255.255.0 | 192.168.2.1 |
| PC19 | PC-PT | 192.168.2.22 | 255.255.255.0 | 192.168.2.1 |
| PC18 | PC-PT | 192.168.2.20 | 255.255.255.0 | 192.168.2.1 |
| PC17 | PC-PT | 192.168.2.19 | 255.255.255.0 | 192.168.2.1 |
| PC16 | PC-PT | 192.168.2.18 | 255.255.255.0 | 192.168.2.1 |
| PC14 | PC-PT | 192.168.2.11 | 255.255.255.0 | 192.168.2.1 |
| PC3  | PC-PT | 192.168.2.3  | 255.255.255.0 | 192.168.2.1 |
| PC11 | PC-PT | 192.168.2.12 | 255.255.255.0 | 192.168.2.1 |
| PC10 | PC-PT | 192.168.2.13 | 255.255.255.0 | 192.168.2.1 |
| PC13 | PC-PT | 192.168.2.14 | 255.255.255.0 | 192.168.2.1 |
| PC12 | PC-PT | 192.168.2.7  | 255.255.255.0 | 192.168.2.1 |
| PC15 | PC-PT | 192.168.2.6  | 255.255.255.0 | 192.168.2.1 |
| Laptop10| Laptop-PT | 192.168.2.17 | 255.255.255.0 | 192.168.2.1 |
| Laptop9 | Laptop-PT | 192.168.2.15 | 255.255.255.0 | 192.168.2.1 |
| Laptop5 | Laptop-PT | 192.168.2.16 | 255.255.255.0 | 192.168.2.1 |
| Laptop4 | Laptop-PT | 192.168.2.27 | 255.255.255.0 | 192.168.2.1 |
| Laptop3 | Laptop-PT | 192.168.2.4  | 255.255.255.0 | 192.168.2.1 |
| Laptop6 | Laptop-PT | 192.168.2.5  | 255.255.255.0 | 192.168.2.1 |
| Laptop7 | Laptop-PT | 192.168.2.8  | 255.255.255.0 | 192.168.2.1 |
| Laptop8 | Laptop-PT | 192.168.2.10 | 255.255.255.0 | 192.168.2.1 |

#### Configuration Notes
Devices Used:
End Devices: 12x PC-PT, 8x Laptop-PT
Switches: 2950-24 Switch (x5)
Connections: Straight Through cables from end devices to switches. Cross Over cables between switches
Configuration Details:
IP Scheme: Manual static IP configuration
Gateway: 192.168.2.1

#### Connectivity Test Evidence 
<img width="1366" height="768" alt="Screenshot (21)" src="https://github.com/user-attachments/assets/35abc1a4-c162-417f-864a-b17121bfe939" />

---

### Hybrid Topology









## Project Reflection
### Challenges Encountered
Devices from different topologies should NOT have the same IP addresses. decided to have devices from different topologies have the same IP address like in the mesh and ring topologies as. later desi
