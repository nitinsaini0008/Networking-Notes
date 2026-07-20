# Network Devices

## About

Network devices are hardware components used to connect computers, transfer data, manage network traffic, and provide communication between different networks.

---

# What are Network Devices?

Network devices help establish communication between devices in a network. Each device performs a specific function based on the OSI Model.

---

# 1. Hub

## Purpose

A Hub connects multiple devices and broadcasts data to every connected device.

## OSI Layer

Layer 1 (Physical Layer)

## Features

- No MAC Address Table
- No Filtering
- Half Duplex
- Broadcasts Data
- Slow Performance

## Advantages

- Low Cost
- Easy to Install

## Disadvantages

- High Network Traffic
- Low Security
- Collision Occurs Frequently

---

# 2. Switch

## Purpose

A Switch connects devices in a LAN and forwards data only to the destination device.

## OSI Layer

Layer 2 (Data Link Layer)

## Features

- Uses MAC Address
- Maintains MAC Address Table
- Full Duplex
- Reduces Collision
- High Speed

## Advantages

- Fast Communication
- Better Security
- Efficient Data Transfer

## Cisco Command

```text
show mac address-table
```

---

# 3. Router

## Purpose

A Router connects different networks and forwards packets using IP addresses.

## OSI Layer

Layer 3 (Network Layer)

## Features

- Uses IP Address
- Connects Different Networks
- Supports Routing Protocols
- Connects LAN to Internet

## Advantages

- Best Path Selection
- Connects Multiple Networks
- Supports NAT and DHCP

## Cisco Command

```text
show ip route
```

---

# 4. Bridge

## Purpose

Connects two LAN segments and filters traffic using MAC addresses.

## OSI Layer

Layer 2 (Data Link Layer)

## Advantages

- Reduces Traffic
- Improves Performance

---

# 5. Repeater

## Purpose

Regenerates weak network signals.

## OSI Layer

Layer 1 (Physical Layer)

## Uses

- Long Distance Communication
- Fiber Networks

---

# 6. Gateway

## Purpose

Acts as an entry and exit point between different networks.

## OSI Layer

Works across multiple OSI layers.

## Example

Home Router connected to the Internet.

---

# 7. Modem

## Purpose

Converts Digital Signals into Analog Signals and vice versa.

## Full Form

Modulator-Demodulator

## Uses

- Internet Connection
- DSL
- Cable Broadband

---

# 8. Access Point (AP)

## Purpose

Provides wireless connectivity to devices.

## Features

- Wi-Fi Access
- Extends Wireless Coverage
- Supports Multiple Devices

---

# 9. Firewall

## Purpose

Protects the network by allowing or blocking traffic based on security rules.

## OSI Layer

Layer 3, Layer 4, and Layer 7 (depending on firewall type)

## Types

- Packet Filtering Firewall
- Stateful Firewall
- Proxy Firewall
- Next Generation Firewall (NGFW)

---

# 10. NIC (Network Interface Card)

## Purpose

Allows a computer to connect to a network.

## Features

- Contains MAC Address
- Wired or Wireless
- Installed in Every Computer

---

# Comparison Table

| Device | OSI Layer | Address Used |
|---------|-----------|--------------|
| Hub | Layer 1 | None |
| Repeater | Layer 1 | None |
| Switch | Layer 2 | MAC Address |
| Bridge | Layer 2 | MAC Address |
| Router | Layer 3 | IP Address |
| Firewall | Layer 3/4/7 | IP, Port, Application |
| Access Point | Layer 2 | MAC Address |
| Gateway | Multiple | IP Address |
| Modem | Layer 1 | None |
| NIC | Layer 2 | MAC Address |

---

# Real-Life Example

Imagine a city road system.

- Hub → Loudspeaker announcing to everyone
- Switch → Security Guard directing people correctly
- Router → GPS selecting the best route
- Firewall → Security Checkpoint
- Access Point → Wi-Fi Hotspot
- Modem → Translator between ISP and Home Network
- NIC → Vehicle Registration Plate

---

# Interview Questions

1. What is the difference between Hub and Switch?
2. Which device works at Layer 3?
3. Which device stores the MAC Address Table?
4. What is the purpose of a Router?
5. What is the full form of Modem?
6. What is the purpose of a Firewall?
7. Difference between Bridge and Switch?
8. What is an Access Point?
9. What is the role of a Gateway?
10. What is a NIC?

---

# Summary

Devices Covered

- Hub
- Switch
- Router
- Bridge
- Repeater
- Gateway
- Modem
- Access Point
- Firewall
- NIC

Topics Covered

- OSI Layers
- Device Functions
- MAC Address
- IP Address
- Cisco Commands
- Comparison Table

**End of File**
