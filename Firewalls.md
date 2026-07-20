# Firewalls

## About

A Firewall is a network security device or software that monitors, filters, and controls incoming and outgoing network traffic based on predefined security rules.

It acts as a barrier between a trusted internal network and an untrusted external network such as the Internet.

---

# What is a Firewall?

A Firewall examines network packets and decides whether to:

- Allow Traffic
- Block Traffic
- Log Traffic
- Monitor Traffic

Example

```
Internet

↓

Firewall

↓

Internal Network
```

---

# Why Use a Firewall?

- Prevent Unauthorized Access
- Protect Against Cyber Attacks
- Control Network Traffic
- Secure Sensitive Data
- Monitor Network Activity

---

# How a Firewall Works

1. Packet arrives at the firewall.
2. Firewall compares the packet with configured rules.
3. Firewall checks:
   - Source IP
   - Destination IP
   - Port Number
   - Protocol
4. Decision is made.
5. Packet is Allowed or Denied.

---

# Types of Firewalls

## 1. Packet Filtering Firewall

Filters packets based on:

- Source IP
- Destination IP
- Port Number
- Protocol

Advantages

- Fast
- Low Resource Usage

Disadvantages

- No Session Awareness
- Limited Security

---

## 2. Stateful Inspection Firewall

Tracks active connections.

Instead of checking only individual packets, it also checks whether the packet belongs to an existing session.

Advantages

- Better Security
- Prevents Unauthorized Sessions

Disadvantages

- Uses More Memory

---

## 3. Proxy Firewall

Acts as an intermediary between the client and the server.

Example

```
Client

↓

Proxy Firewall

↓

Internet
```

Advantages

- Hides Internal Network
- Content Filtering
- Better Privacy

Disadvantages

- Higher Latency

---

## 4. Next Generation Firewall (NGFW)

Modern firewall with advanced security features.

Features

- Deep Packet Inspection (DPI)
- Intrusion Prevention System (IPS)
- Application Control
- Malware Detection
- SSL Inspection
- User Identity Awareness

Examples

- Cisco Firepower
- Palo Alto
- Fortinet FortiGate
- Check Point

---

# Firewall Deployment Types

## Network Firewall

Protects an entire network.

Installed between the LAN and the Internet.

---

## Host-Based Firewall

Installed on an individual computer.

Examples

- Windows Defender Firewall
- Linux firewalld
- UFW (Ubuntu)

---

# Access Control List (ACL)

An ACL is a list of rules used to allow or deny network traffic.

ACLs are commonly used on Cisco routers and switches.

---

# Types of ACL

## Standard ACL

Filters traffic based only on the Source IP Address.

ACL Range

```
1–99
```

Example

```bash
access-list 10 permit 192.168.1.0 0.0.0.255
```

---

## Extended ACL

Filters traffic based on:

- Source IP
- Destination IP
- Protocol
- Port Number

ACL Range

```
100–199
```

Example

```bash
access-list 100 permit tcp any any eq 80
```

---

# Cisco ACL Configuration

Create Standard ACL

```bash
access-list 10 permit 192.168.1.0 0.0.0.255
```

Apply ACL

```bash
interface GigabitEthernet0/0

ip access-group 10 in
```

Create Extended ACL

```bash
access-list 100 permit tcp any any eq 443
```

---

# Firewall Rule Example

| Source | Destination | Port | Action |
|---------|-------------|------|--------|
| Any | Web Server | 80 | Allow |
| Any | Web Server | 443 | Allow |
| Any | Internal Network | Any | Deny |

---

# Verification Commands

Show ACL

```bash
show access-lists
```

Show Running Configuration

```bash
show running-config
```

Show Interface

```bash
show ip interface
```

---

# Advantages

- Protects Against Unauthorized Access
- Filters Malicious Traffic
- Improves Network Security
- Supports Access Control
- Monitors Network Activity

---

# Disadvantages

- Incorrect Rules May Block Legitimate Traffic
- Requires Proper Configuration
- Advanced Firewalls Can Be Expensive

---

# Real-Life Example

Imagine a security guard at the entrance of a company.

The guard checks:

- Identity Card
- Visitor Purpose
- Entry Permission

If everything is valid, entry is allowed.

Otherwise, access is denied.

A Firewall works in the same way by checking network traffic before allowing it into the network.

---

# Interview Questions

1. What is a Firewall?
2. Why is a Firewall used?
3. What is the difference between Packet Filtering and Stateful Inspection Firewalls?
4. What is a Proxy Firewall?
5. What is an NGFW?
6. What is an ACL?
7. What is the difference between Standard ACL and Extended ACL?
8. Which Cisco command displays ACLs?
9. What is a Host-Based Firewall?
10. Name some popular Firewall vendors.

---

# Summary

Topics Covered

- Firewall
- Packet Filtering Firewall
- Stateful Inspection Firewall
- Proxy Firewall
- Next Generation Firewall (NGFW)
- Network Firewall
- Host-Based Firewall
- ACL
- Cisco ACL Configuration
- Verification Commands

Cisco Commands

- access-list
- ip access-group
- show access-lists
- show running-config
- show ip interface

**End of File**
