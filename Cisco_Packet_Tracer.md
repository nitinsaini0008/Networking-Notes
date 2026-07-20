# Cisco Packet Tracer

## About

Cisco Packet Tracer is a network simulation software developed by Cisco. It allows students and network engineers to design, configure, simulate, and troubleshoot computer networks without using physical networking devices.

---

# What is Cisco Packet Tracer?

Cisco Packet Tracer provides a virtual environment to build and test network topologies using Cisco devices.

Example

```
PC1

↓

Switch

↓

Router

↓

Internet
```

Everything is simulated virtually.

---

# Why Use Cisco Packet Tracer?

- Learn Networking
- Practice Cisco CLI
- Build Network Topologies
- Test Configurations
- Prepare for CCNA
- Troubleshoot Networks

---

# Features

- Drag-and-Drop Interface
- Cisco IOS CLI
- Real-Time Simulation
- Simulation Mode
- Multiple Device Support
- Wireless Network Simulation
- IoT Device Support

---

# Devices Available

## End Devices

- PC
- Laptop
- Server
- Printer
- IP Phone
- Tablet
- Smartphone

---

## Network Devices

- Router
- Switch
- Hub
- Wireless Router
- Access Point
- Firewall
- Modem

---

## Connections

- Copper Straight-Through
- Copper Cross-Over
- Fiber Cable
- Console Cable
- Serial Cable

---

# Packet Tracer Modes

## 1. Real-Time Mode

Network operates normally without packet-by-packet analysis.

Used for:

- Configuration
- Testing
- Practice

---

## 2. Simulation Mode

Allows users to observe packets moving through the network step by step.

Used for:

- Packet Analysis
- Troubleshooting
- Learning Protocols

---

# Basic Topology Example

```
PC0

↓

Switch0

↓

Router0

↓

Server0
```

---

# Basic Router Configuration

Enter Privileged Mode

```bash
enable
```

Enter Global Configuration Mode

```bash
configure terminal
```

Configure Interface

```bash
interface GigabitEthernet0/0
```

Assign IP Address

```bash
ip address 192.168.1.1 255.255.255.0
```

Enable Interface

```bash
no shutdown
```

Exit

```bash
exit
```

Save Configuration

```bash
copy running-config startup-config
```

---

# Basic Switch Configuration

Enter Configuration Mode

```bash
enable

configure terminal
```

Set Hostname

```bash
hostname Switch1
```

Configure VLAN

```bash
vlan 10

name HR
```

Assign Port

```bash
interface FastEthernet0/1

switchport mode access

switchport access vlan 10
```

Save Configuration

```bash
copy running-config startup-config
```

---

# PC Configuration

Desktop

↓

IP Configuration

Fill in:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server

Example

```
IP Address

192.168.1.10

Subnet Mask

255.255.255.0

Gateway

192.168.1.1

DNS

8.8.8.8
```

---

# Testing Connectivity

Ping Gateway

```bash
ping 192.168.1.1
```

Ping Another PC

```bash
ping 192.168.1.20
```

---

# Useful Cisco Commands

Show Running Configuration

```bash
show running-config
```

Show IP Interface Brief

```bash
show ip interface brief
```

Show Routing Table

```bash
show ip route
```

Show VLANs

```bash
show vlan brief
```

Show MAC Address Table

```bash
show mac address-table
```

Show Interface Status

```bash
show interfaces status
```

---

# Common Packet Tracer Labs

- Basic LAN Setup
- Router Configuration
- Switch Configuration
- VLAN Configuration
- Inter-VLAN Routing
- DHCP Server
- DNS Server
- FTP Server
- NAT Configuration
- ACL Configuration
- Static Routing
- Dynamic Routing (RIP, OSPF, EIGRP)

---

# Advantages

- Free for Cisco Networking Academy Students
- Easy to Learn
- No Physical Hardware Required
- Supports Real Cisco CLI
- Excellent for CCNA Practice

---

# Limitations

- Simulation Only
- Does Not Support Every Cisco Feature
- Not Suitable for Large Enterprise Networks
- Limited Compared to Real Cisco Hardware

---

# Real-Life Example

Imagine learning to drive using a driving simulator.

You can practice:

- Steering
- Braking
- Parking

without risking a real vehicle.

Similarly, Cisco Packet Tracer lets you practice networking without using real routers and switches.

---

# Interview Questions

1. What is Cisco Packet Tracer?
2. Why is Cisco Packet Tracer used?
3. What is the difference between Real-Time Mode and Simulation Mode?
4. Which devices are available in Packet Tracer?
5. How do you configure an IP address on a router?
6. Which command displays interface information?
7. Which command saves the running configuration?
8. Which command displays VLAN information?
9. How do you test connectivity between two devices?
10. Is Cisco Packet Tracer suitable for CCNA preparation?

---

# Summary

Topics Covered

- Cisco Packet Tracer
- Features
- Devices
- Real-Time Mode
- Simulation Mode
- Router Configuration
- Switch Configuration
- PC Configuration
- Connectivity Testing
- Common Labs

Common Cisco Commands

- enable
- configure terminal
- show running-config
- show ip interface brief
- show ip route
- show vlan brief
- show mac address-table
- copy running-config startup-config
- ping

**End of File**
