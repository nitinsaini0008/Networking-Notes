# DHCP (Dynamic Host Configuration Protocol)

## About

Dynamic Host Configuration Protocol (DHCP) is a network management protocol that automatically assigns IP addresses and other network configuration information to devices on a network.

---

# What is DHCP?

DHCP automatically provides:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server
- Lease Time

Without DHCP, every device must be configured manually.

---

# Why Use DHCP?

- Automatic IP Assignment
- Reduces Human Errors
- Saves Time
- Easy Network Management
- Prevents IP Address Conflicts

---

# DHCP Components

## DHCP Server

Assigns IP addresses to clients.

Examples

- Windows Server
- Linux Server
- Cisco Router

---

## DHCP Client

Requests an IP address.

Examples

- Laptop
- Desktop
- Mobile Phone
- Printer

---

# DHCP Process (DORA)

## Step 1 - Discover

Client broadcasts a DHCP Discover message.

```
Client → Broadcast → DHCP Discover
```

---

## Step 2 - Offer

DHCP Server offers an available IP address.

```
Server → DHCP Offer
```

---

## Step 3 - Request

Client requests the offered IP address.

```
Client → DHCP Request
```

---

## Step 4 - Acknowledge

Server confirms the IP assignment.

```
Server → DHCP ACK
```

---

# DORA Diagram

```
Client
   │
   │ DHCP Discover
   ▼
DHCP Server
   ▲
   │ DHCP Offer
   │
Client
   │ DHCP Request
   ▼
DHCP Server
   ▲
   │ DHCP ACK
   │
Client Receives IP Address
```

---

# DHCP Lease

A Lease is the amount of time a client can use an assigned IP address.

Example

```
24 Hours
```

After the lease expires, the client renews the IP address.

---

# DHCP Scope

A DHCP Scope is the range of IP addresses available for assignment.

Example

```
192.168.1.10

to

192.168.1.200
```

---

# DHCP Reservation

A Reservation assigns the same IP address to a specific device using its MAC Address.

Used For

- Servers
- Printers
- CCTV
- Network Devices

---

# DHCP Relay Agent

Used when the DHCP Server is located on another network.

Cisco Command

```bash
ip helper-address 192.168.1.10
```

---

# Cisco DHCP Configuration

Enable Configuration

```bash
configure terminal
```

Create DHCP Pool

```bash
ip dhcp pool OFFICE
```

Network

```bash
network 192.168.10.0 255.255.255.0
```

Default Gateway

```bash
default-router 192.168.10.1
```

DNS Server

```bash
dns-server 8.8.8.8
```

Exit

```bash
exit
```

Exclude Reserved Addresses

```bash
ip dhcp excluded-address 192.168.10.1 192.168.10.20
```

---

# Verification Commands

Display DHCP Pool

```bash
show ip dhcp pool
```

Display DHCP Bindings

```bash
show ip dhcp binding
```

Display Running Configuration

```bash
show running-config
```

---

# Advantages

- Automatic Configuration
- Faster Deployment
- Centralized Management
- Prevents Duplicate IP Addresses
- Easy Maintenance

---

# Disadvantages

- DHCP Server Failure Affects Clients
- Security Risks if Unauthorized DHCP Exists
- Lease Management Required

---

# Real-Life Example

Imagine a hotel reception.

Guest → Requests a room.

Reception → Assigns an available room number.

After checkout, the room becomes available for another guest.

Similarly,

Client → Requests IP Address.

DHCP Server → Assigns Available IP.

---

# Interview Questions

1. What is DHCP?
2. What is the full form of DHCP?
3. Explain the DORA process.
4. What is a DHCP Lease?
5. What is a DHCP Scope?
6. What is DHCP Reservation?
7. What is the purpose of a DHCP Relay Agent?
8. Which Cisco command creates a DHCP Pool?
9. Which command displays DHCP bindings?
10. What happens if the DHCP Server is unavailable?

---

# Summary

Topics Covered

- DHCP
- DHCP Server
- DHCP Client
- DORA Process
- DHCP Lease
- DHCP Scope
- DHCP Reservation
- DHCP Relay Agent
- Cisco DHCP Configuration
- Verification Commands

Cisco Commands

- ip dhcp pool
- network
- default-router
- dns-server
- ip dhcp excluded-address
- show ip dhcp pool
- show ip dhcp binding

**End of File**
