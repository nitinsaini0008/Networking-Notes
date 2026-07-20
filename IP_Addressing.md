# IP Addressing

## About

IP Addressing is the process of assigning a unique numerical address to every device connected to a network. It enables communication between computers, servers, routers, and other network devices.

---

# What is an IP Address?

An IP (Internet Protocol) Address is a unique identifier assigned to every device connected to a network.

Example

```text
192.168.1.10
```

---

# Versions of IP

| Version | Size | Example |
|---------|------|----------|
| IPv4 | 32-bit | 192.168.1.1 |
| IPv6 | 128-bit | 2001:db8::1 |

---

# IPv4 Address

IPv4 consists of **32 bits** divided into **4 octets**.

Example

```text
192.168.1.100
```

Each octet ranges from:

```text
0 - 255
```

---

# IPv6 Address

IPv6 consists of **128 bits** divided into **8 hexadecimal blocks**.

Example

```text
2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

Short Form

```text
2001:db8:85a3::8a2e:370:7334
```

---

# IPv4 Address Classes

| Class | Range | Default Mask | Purpose |
|--------|----------------|---------------|----------------|
| A | 1 – 126 | 255.0.0.0 | Large Networks |
| B | 128 – 191 | 255.255.0.0 | Medium Networks |
| C | 192 – 223 | 255.255.255.0 | Small Networks |
| D | 224 – 239 | Multicast | Multicast Traffic |
| E | 240 – 255 | Reserved | Research |

---

# Private IP Address Ranges

| Class | Range |
|---------|-----------------------|
| A | 10.0.0.0 – 10.255.255.255 |
| B | 172.16.0.0 – 172.31.255.255 |
| C | 192.168.0.0 – 192.168.255.255 |

---

# Public IP Address

A Public IP Address is assigned by an Internet Service Provider (ISP) and is accessible over the Internet.

Example

```text
49.36.210.25
```

---

# Loopback Address

Used for testing the local machine.

IPv4

```text
127.0.0.1
```

IPv6

```text
::1
```

---

# APIPA Address

APIPA (Automatic Private IP Addressing) is assigned automatically when a DHCP server is unavailable.

Range

```text
169.254.0.0 – 169.254.255.255
```

---

# Network Address

Represents the entire network.

Example

```text
192.168.1.0/24
```

---

# Broadcast Address

Used to send data to every device in the network.

Example

```text
192.168.1.255
```

---

# Subnet Mask

A subnet mask separates the Network ID from the Host ID.

Example

```text
255.255.255.0
```

CIDR Notation

```text
/24
```

---

# CIDR Examples

| CIDR | Subnet Mask |
|-------|----------------|
| /8 | 255.0.0.0 |
| /16 | 255.255.0.0 |
| /24 | 255.255.255.0 |
| /25 | 255.255.255.128 |
| /26 | 255.255.255.192 |
| /27 | 255.255.255.224 |
| /28 | 255.255.255.240 |
| /29 | 255.255.255.248 |
| /30 | 255.255.255.252 |

---

# Network ID vs Host ID

Example

```text
IP Address : 192.168.10.25
Subnet Mask: 255.255.255.0
```

Network ID

```text
192.168.10.0
```

Host ID

```text
25
```

---

# Static IP

A manually configured IP address that remains the same.

Examples

- Server
- Printer
- CCTV
- Router

---

# Dynamic IP

An IP address assigned automatically by a DHCP server.

Examples

- Mobile Phone
- Laptop
- Home PC

---

# Advantages of IPv6

- Huge Address Space
- Better Security
- Faster Routing
- No NAT Required
- Auto Configuration

---

# Interview Questions

1. What is an IP Address?
2. Difference between IPv4 and IPv6?
3. What is a Private IP Address?
4. What is a Public IP Address?
5. What is APIPA?
6. What is Loopback Address?
7. What is CIDR?
8. Difference between Static and Dynamic IP?
9. What is a Subnet Mask?
10. Which IP Classes are used in networking?

---

# Summary

Topics Covered

- IPv4
- IPv6
- IP Classes
- Private IP
- Public IP
- Loopback
- APIPA
- Network Address
- Broadcast Address
- Subnet Mask
- CIDR
- Static IP
- Dynamic IP

**End of File**
