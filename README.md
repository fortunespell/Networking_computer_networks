# Network Topology Configurations

This repository contains multiple network topology diagrams created using Cisco Packet Tracer. These diagrams are designed to demonstrate common network setups used in small offices, home networks, and larger corporate environments. Each topology highlights key networking concepts, including device interconnectivity, routing, switching, and network segmentation.

## Table of Contents
- [Overview](#overview)
- [Diagrams and Descriptions](#diagrams-and-descriptions)
  - [1. Basic Router-Switch-PC Network](#1-basic-router-switch-pc-network)
  - [2. Simple Router-Switch-PC Network](#2-simple-router-switch-pc-network)
  - [3. Advanced Multi-Router Network](#3-advanced-multi-router-network)
- [How to Use](#how-to-use)
- [Getting Started](#getting-started)
- [Requirements](#requirements)
- [License](#license)

## Overview

Networking is essential for communication between devices, and understanding how routers, switches, and computers (PCs) interact within different topologies is crucial for building and managing any network. This repository features several common networking topologies:

1. **Basic Router-Switch-PC Network**: A fundamental example of how devices in a small office or home environment communicate via a router and a switch.
2. **Simple Router-Switch-PC Network**: A compact LAN configuration where multiple devices share the same local switch and communicate with a single router.
3. **Advanced Multi-Router Network**: A complex, corporate-style network featuring multiple routers, subnets, and switches for optimal traffic management and network segmentation.

Each diagram provides an introduction to the networking devices and topologies involved, and demonstrates how to configure routers, switches, and PCs for basic communication and routing.

## Diagrams and Descriptions

### 1. Basic Router-Switch-PC Network

#### **Overview:**
This diagram represents a simple network structure, commonly seen in small offices or homes, with:
- **2 PCs**: PC0, PC1
- **2 Routers**: Router0, Router1
- **1 Switch**: Switch0

#### **Description:**
- **PC0** is connected to **Switch0**, which is further connected to **Router0**.
- **Router0** and **Router1** are connected via a serial or fast Ethernet WAN link (shown in red).
- **PC1** is directly connected to **Router1**.

#### **Network Role and Functionality:**
- **Router0** manages local area network (LAN) traffic, allowing devices connected to **Switch0** (e.g., PC0) to communicate.
- **Router1** extends the network, simulating an external network (or another subnet), which may represent an ISP or an external office. **PC1** represents a device from this external network.
- The **Switch** allows multiple devices to share the same network, optimizing LAN traffic by directing packets to the correct device based on MAC addresses.

#### **Use Case**:
This topology is ideal for learning basic routing principles, demonstrating how LANs and WANs interconnect, and setting up small-scale networks in offices or home environments. It can also be used to simulate external connectivity (like an ISP connection) through Router1.

![image](https://github.com/user-attachments/assets/24933e20-ed2f-4587-be92-de849119d2d0)

---

### 2. Simple Router-Switch-PC Network (VLAN)

#### **Overview:**
This topology involves a local network where:
- **2 PCs**: PC2, PC3
- **1 Router**: Router2
- **1 Switch**: Switch4

#### **Description:**
- **PC2** and **PC3** are connected to **Switch4**, which acts as the intermediary for communication within the network.
- **Router2** is connected to **Switch4** and provides gateway services to connect this internal network to an external network (such as the internet or another subnet).

#### **Network Role and Functionality:**
- The switch enables communication between **PC2** and **PC3** at the data link layer (Layer 2 of the OSI model). 
- **Router2** operates at the network layer (Layer 3), routing packets between this local network and external networks.

#### **Use Case:**
This topology represents a typical small-scale local area network (LAN) where multiple devices (PC2 and PC3) need to communicate with each other internally, while **Router2** provides connectivity to the outside world. This setup is widely used in homes and small businesses where basic networking infrastructure (router and switch) is sufficient for daily communication and internet access.

![image](https://github.com/user-attachments/assets/e12c843f-f4bc-451d-8369-a7e156dc451c)

---

### 3. Advanced Multi-Router Network

#### **Overview:**
A more complex network topology involving:
- **6 PCs**: PC0, PC1, PC2, PC3, PC4, PC5
- **3 Routers**: Router0, Router1, Router2
- **2 Switches**: Switch0, Switch1

#### **Description:**
- PCs are distributed and connected to either **Switch0** or **Switch1**.
- **Router0**, **Router1**, and **Router2** form a WAN with serial connections (in red), creating a triangular backbone for inter-router communication.
- **Switch0** connects **PC0**, **PC1**, **PC4**, and **PC5**.
- **Switch1** connects **PC2** and **PC3**.

#### **Network Role and Functionality:**
- The network is designed for interdepartmental communication in a larger corporate environment. Each switch can represent a department, with **Router0**, **Router1**, and **Router2** managing traffic between different subnets or geographical locations.
- Redundant links between routers ensure network reliability, as traffic can be rerouted in case one link fails, demonstrating the resilience of a mesh network.
  
#### **Use Case:**
This topology is suitable for large organizations or enterprises where multiple departments or offices are connected. Each router manages specific subnets, and the network configuration ensures redundancy and fault tolerance, enabling smooth internal and external communication. This network can handle larger data flows and different VLANs for each department.

![image](https://github.com/user-attachments/assets/e654dff8-e3d5-4f0f-b64c-2b73b5eb7fbd)

---

## How to Use

1. **Network Configuration**: You can manually configure IP addresses, subnet masks, and gateways for the PCs and routers.
2. **Routing Protocols**: Experiment with routing protocols like RIP, OSPF, or EIGRP for dynamic routing between the routers.
3. **Packet Flow Simulation**: Use Cisco Packet Tracer’s simulation mode to trace the path of packets between devices, and observe how routing and switching operate.
4. **Troubleshooting**: Practice troubleshooting with ping tests, examining ARP tables, and inspecting routing tables on routers to learn how data flows through the network.

---

## Getting Started

To simulate and experiment with these network topologies:

1. **Install Cisco Packet Tracer**: [Download Packet Tracer](https://www.netacad.com/courses/packet-tracer) and follow the installation guide for your operating system.
2. **Clone this Repository**: Clone or download this repository to your local machine.
   ```bash
   git clone https://github.com/your-username/network-topology-configurations.git

   
---

This version provides more details on the diagrams' roles, potential configurations, use cases, and how to engage with the network topologies. Would you like to modify anything further or add additional sections?

