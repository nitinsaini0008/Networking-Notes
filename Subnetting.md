# Subnetting

## About

Subnetting is the process of dividing a large network into multiple smaller networks (subnets). It improves network performance, enhances security, and efficiently utilizes IP addresses.

---

# What is Subnetting?

Subnetting divides one large network into smaller logical networks.

Example

```
192.168.1.0/24
```

can be divided into:

```
192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26
```

---

# Why Do We Use Subnetting?

- Efficient IP Address Utilization
- Better Network Performance
- Reduced Broadcast Traffic
- Improved Security
- Easier Network Management

---

# Basic Terms

## Network Address

First IP of a subnet.

Example

```
192.168.1.0
```

---

## Broadcast Address

Last IP of a subnet.

Example

```
192.168.1.255
```

---

## Host Address

Usable IP addresses between the Network Address and Broadcast Address.

Example

```
192.168.1.1
to
192.168.1.254
```

---

# CIDR Notation

| CIDR | Subnet Mask | Hosts |
|------|-----------------|------|
| /24 | 255.255.255.0 | 254 |
| /25 | 255.255.255.128 | 126 |
| /26 | 255.255.255.192 | 62 |
| /27 | 255.255.255.224 | 30 |
| /28 | 255.255.255.240 | 14 |
| /29 | 255.255.255.248 | 6 |
| /30 | 255.255.255.252 | 2 |

---

# Formula

## Number of Subnets

```
2^n
```

Where:

```
n = Borrowed Bits
```

---

## Number of Hosts

```
2^h - 2
```

Where

```
h = Host Bits
```

---

# Example 1

Network

```
192.168.1.0/24
```

Convert into

```
/26
```

Borrowed Bits

```
2
```

Subnets

```
2² = 4
```

Hosts

```
2⁶ - 2 = 62
```

---

# Subnet Table (/26)

| Network | First Host | Last Host | Broadcast |
|---------|------------|-----------|-----------|
|192.168.1.0|192.168.1.1|192.168.1.62|192.168.1.63|
|192.168.1.64|192.168.1.65|192.168.1.126|192.168.1.127|
|192.168.1.128|192.168.1.129|192.168.1.190|192.168.1.191|
|192.168.1.192|192.168.1.193|192.168.1.254|192.168.1.255|

---

# Example 2

Subnet

```
10.0.0.0/16
```

Convert into

```
/24
```

Subnets

```
256
```

Hosts per Subnet

```
254
```

---

# Binary Representation

Example

```
255.255.255.0
```

Binary

```
11111111.11111111.11111111.00000000
```

---

# VLSM

VLSM stands for

```
Variable Length Subnet Mask
```

It allows different subnet sizes according to requirements.

Example

- HR → 20 Hosts
- Sales → 50 Hosts
- IT → 100 Hosts

Each department can have a different subnet size.

---

# FLSM

FLSM stands for

```
Fixed Length Subnet Mask
```

All subnets have the same size.

---

# Advantages

- Efficient IP Usage
- Better Security
- Reduced Congestion
- Easy Troubleshooting
- Better Performance

---

# Disadvantages

- More Planning Required
- Configuration Complexity
- Requires Subnetting Knowledge

---

# Interview Questions

1. What is subnetting?
2. Why is subnetting used?
3. Difference between VLSM and FLSM?
4. What is CIDR?
5. What is a subnet mask?
6. What is the Network Address?
7. What is the Broadcast Address?
8. How many hosts are available in /27?
9. How many hosts are available in /30?
10. What is the formula to calculate hosts?

---

# Summary

Topics Covered

- Subnetting
- CIDR
- Network Address
- Broadcast Address
- Host Address
- VLSM
- FLSM
- Binary
- Subnet Calculations

**End of File**
