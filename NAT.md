# NAT (Network Address Translation)

## About

Network Address Translation (NAT) is a technique used by routers to translate private IP addresses into public IP addresses and vice versa. NAT allows multiple devices in a private network to access the Internet using one or more public IP addresses.

---

# What is NAT?

NAT modifies the source or destination IP address of packets as they pass through a router.

Example

```
Private Network

PC1 (192.168.1.10)
PC2 (192.168.1.11)
PC3 (192.168.1.12)

        │
        ▼

     NAT Router

Public IP
203.0.113.10

        │
        ▼

     Internet
```

---

# Why Use NAT?

- Conserves Public IPv4 Addresses
- Allows Multiple Devices to Share One Public IP
- Hides Internal Network Structure
- Improves Security
- Reduces IPv4 Address Exhaustion

---

# NAT Terminology

## Inside Local Address

Private IP address assigned to a device inside the local network.

Example

```
192.168.1.10
```

---

## Inside Global Address

Public IP address representing an inside device on the Internet.

Example

```
203.0.113.10
```

---

## Outside Local Address

The destination address of an external device as seen from the internal network.

---

## Outside Global Address

The actual public IP address of the external destination.

Example

```
142.250.183.110
```

---

# Types of NAT

## 1. Static NAT

One private IP is permanently mapped to one public IP.

Example

```
192.168.1.10

↓

203.0.113.10
```

### Advantages

- Fixed Public IP
- Suitable for Web Servers

### Disadvantages

- Requires One Public IP per Device

---

## 2. Dynamic NAT

Private IP addresses are translated using a pool of available public IP addresses.

Example

```
192.168.1.10

↓

203.0.113.10

192.168.1.11

↓

203.0.113.11
```

### Advantages

- Automatic Allocation
- Better than Static NAT

### Disadvantages

- Limited by Public IP Pool Size

---

## 3. PAT (Port Address Translation)

Also called NAT Overload.

Multiple private devices share a single public IP using different port numbers.

Example

```
192.168.1.10:5001

↓

203.0.113.10:5001

192.168.1.11:5002

↓

203.0.113.10:5002
```

### Advantages

- Saves Public IP Addresses
- Most Common NAT Type
- Ideal for Home and Office Networks

---

# NAT Comparison

| Feature | Static NAT | Dynamic NAT | PAT |
|---------|------------|-------------|-----|
| Public IP Required | One per Device | Pool of IPs | One Public IP |
| Mapping | Fixed | Dynamic | Port-Based |
| Internet Sharing | No | Limited | Yes |
| Common Usage | Servers | Medium Networks | Home & Enterprise |

---

# Cisco NAT Configuration

## Configure Inside Interface

```bash
interface GigabitEthernet0/0
ip nat inside
```

---

## Configure Outside Interface

```bash
interface GigabitEthernet0/1
ip nat outside
```

---

## Configure PAT

```bash
access-list 1 permit 192.168.1.0 0.0.0.255

ip nat inside source list 1 interface GigabitEthernet0/1 overload
```

---

## Configure Static NAT

```bash
ip nat inside source static 192.168.1.10 203.0.113.10
```

---

# Verification Commands

Display NAT Translations

```bash
show ip nat translations
```

Display NAT Statistics

```bash
show ip nat statistics
```

Display Running Configuration

```bash
show running-config
```

---

# Advantages

- Conserves IPv4 Addresses
- Enhances Security
- Enables Internet Access
- Easy to Deploy
- Supports Large Networks

---

# Disadvantages

- Slight Processing Overhead
- Some Applications May Require NAT Configuration
- End-to-End Connectivity Can Be More Complex

---

# Real-Life Example

Imagine an apartment building.

- Every apartment has its own flat number (Private IP).
- The building has one main street address (Public IP).

People outside know only the building's address, while the receptionist (NAT Router) directs visitors to the correct apartment.

---

# Interview Questions

1. What is NAT?
2. Why is NAT used?
3. What is the difference between Static NAT and Dynamic NAT?
4. What is PAT?
5. What is NAT Overload?
6. What is an Inside Local Address?
7. What is an Inside Global Address?
8. Which NAT type is commonly used in home networks?
9. Which command displays NAT translations?
10. What are the advantages of NAT?

---

# Summary

Topics Covered

- NAT
- Static NAT
- Dynamic NAT
- PAT (NAT Overload)
- Inside Local Address
- Inside Global Address
- Outside Local Address
- Outside Global Address
- Cisco NAT Configuration
- Verification Commands

Cisco Commands

- ip nat inside
- ip nat outside
- ip nat inside source static
- ip nat inside source list
- show ip nat translations
- show ip nat statistics

**End of File**
