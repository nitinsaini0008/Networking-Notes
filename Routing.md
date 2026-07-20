# Routing

## About

Routing is the process of selecting the best path for forwarding data packets from a source network to a destination network. Routers use routing tables and routing protocols to make forwarding decisions.

---

# What is Routing?

Routing allows communication between different networks using IP addresses.

Example

```
PC1 → Switch → Router → Internet → Router → PC2
```

---

# Types of Routing

## 1. Static Routing

Static Routing is configured manually by the network administrator.

### Advantages

- Secure
- Low CPU Usage
- Easy for Small Networks

### Disadvantages

- Manual Configuration
- Difficult to Manage in Large Networks

### Cisco Command

```bash
ip route 192.168.2.0 255.255.255.0 10.0.0.2
```

---

## 2. Dynamic Routing

Dynamic Routing automatically learns routes using routing protocols.

### Advantages

- Automatic Updates
- Suitable for Large Networks
- Less Manual Work

### Disadvantages

- Higher CPU Usage
- More Complex Configuration

---

# Routing Protocols

## RIP (Routing Information Protocol)

### Features

- Distance Vector Protocol
- Maximum 15 Hops
- Metric = Hop Count
- Slow Convergence

### Command

```bash
router rip
version 2
network 192.168.1.0
```

---

## OSPF (Open Shortest Path First)

### Features

- Link State Protocol
- Fast Convergence
- Uses Cost Metric
- Suitable for Large Networks

### Command

```bash
router ospf 1
network 192.168.1.0 0.0.0.255 area 0
```

---

## EIGRP (Enhanced Interior Gateway Routing Protocol)

### Features

- Cisco Proprietary (originally)
- Fast Convergence
- Uses Bandwidth and Delay
- Hybrid Routing Protocol

### Command

```bash
router eigrp 100
network 192.168.1.0
no auto-summary
```

---

# Default Route

A default route is used when no specific route exists.

### Cisco Command

```bash
ip route 0.0.0.0 0.0.0.0 192.168.1.1
```

---

# Routing Table

A Routing Table stores all known routes.

### Cisco Command

```bash
show ip route
```

Example

```
C 192.168.1.0/24
S 192.168.2.0/24
R 192.168.3.0/24
O 192.168.4.0/24
```

---

# Route Types

| Code | Meaning |
|------|---------|
| C | Connected |
| S | Static |
| R | RIP |
| O | OSPF |
| D | EIGRP |

---

# Administrative Distance

| Route | AD |
|--------|----|
| Connected | 0 |
| Static | 1 |
| EIGRP | 90 |
| OSPF | 110 |
| RIP | 120 |

---

# Routing Metrics

| Protocol | Metric |
|-----------|--------|
| RIP | Hop Count |
| OSPF | Cost |
| EIGRP | Bandwidth & Delay |

---

# Routing Process

1. Packet Arrives
2. Router Checks Routing Table
3. Best Route Selected
4. Packet Forwarded
5. Destination Reached

---

# Advantages

- Connects Multiple Networks
- Best Path Selection
- Efficient Traffic Management
- Supports Internet Communication

---

# Disadvantages

- Complex Configuration
- Requires Skilled Administrator
- Hardware Cost

---

# Real-Life Example

Imagine Google Maps.

- Destination → IP Address
- Roads → Network Links
- GPS → Router
- Best Route → Routing Protocol

---

# Interview Questions

1. What is Routing?
2. Difference between Static and Dynamic Routing?
3. What is RIP?
4. What is OSPF?
5. What is EIGRP?
6. What is Administrative Distance?
7. What is a Default Route?
8. Which protocol uses Hop Count?
9. Which protocol uses Cost?
10. Which command displays the Routing Table?

---

# Summary

Topics Covered

- Static Routing
- Dynamic Routing
- RIP
- OSPF
- EIGRP
- Routing Table
- Default Route
- Administrative Distance
- Routing Metrics

Cisco Commands

- show ip route
- ip route
- router rip
- router ospf
- router eigrp

**End of File**
