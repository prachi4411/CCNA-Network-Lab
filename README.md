# CCNA-Network-Lab
# 🖧 CCNA Network Lab: ACCOUNTS ↔ DELIVERY
**Design and Implementation of a Simple Networking Project #1**

![Network Topology](Diagrams/Network_Topology.jpg)

## 📝 Project Description
Design a network in Cisco Packet Tracer to connect the ACCOUNTS and DELIVERY departments with the following requirements:

- Each department should contain at least two PCs.
- Appropriate number of switches and routers should be used in the network.
- Using the given network `192.168.40.0`, all interfaces should be configured with correct IP addresses, subnet masks, and gateways.
- All devices in the network should be connected using appropriate cables.
- Test communication between devices in both ACCOUNTS and DELIVERY departments.

## 🗺️ Topology
- 2 departments: ACCOUNTS and DELIVERY
- Each department has 2 PCs connected to a switch
- Main-Router connects the two switches

## 📡 IP Addressing
| Device        | Interface/PC    | IP Address      | Subnet Mask     | Default Gateway |
|---------------|-----------------|-----------------|-----------------|-----------------|
| Main-Router   | G0/1 (Accounts) | 192.168.40.1    | 255.255.255.128 | -               |
| Main-Router   | G0/2 (Delivery) | 192.168.40.129  | 255.255.255.128 | -               |
| Accounts-PC1  | Fa0/1           | 192.168.40.5    | 255.255.255.128 | 192.168.40.1    |
| Accounts-PC2  | Fa0/2           | 192.168.40.6    | 255.255.255.128 | 192.168.40.1    |
| Delivery-PC1  | Fa0/1           | 192.168.40.135  | 255.255.255.128 | 192.168.40.129  |
| Delivery-PC2  | Fa0/2           | 192.168.40.136  | 255.255.255.128 | 192.168.40.129  |

## 🛠️ Technologies Implemented
- Creating a Simple Network using a Router and Access Layer Switch
- Connecting two Networks using a Router
- Subnetting and IP Addressing
- Assigning IP Addresses to the Router's interfaces
- Static IP Address allocation to Host Devices
- Testing and Verifying Network Communication
- Router-to-Switch connectivity
- Switch-to-PC access ports
- Port-security with sticky MACs
- Static IP addressing
- Ping tests between all devices

## ✅ Test Results
- All PCs in ACCOUNTS can ping each other ✅
- All PCs in DELIVERY can ping each other ✅
- ACCOUNTS ↔ DELIVERY communication via Main-Router ✅

## 📁 Files in this Repository
- `Configs` – Router and Switch Configs  
- `Diagrams` – Network Diagrams 
- `Images` – Ping_Test  
- `PKT` – Packet Tracer Project File  


![Ping Test Example](Images/Ping_Test.png)
