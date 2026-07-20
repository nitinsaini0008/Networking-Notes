# Switching

## About

Switching is the process of forwarding data frames from one device to another within the same Local Area Network (LAN). A switch uses MAC addresses to identify the destination device and sends data only to the intended receiver.

---

# What is Switching?

Switching is a Layer 2 technology that allows efficient communication between devices connected to a LAN.

Example

```
PC1 → Switch → PC2
```

---

# What is a Switch?

A Switch is a networking device that connects multiple devices in a LAN and forwards data using MAC Addresses.

OSI Layer

```
Layer 2 (Data Link Layer)
```

Some Layer 3 switches can also perform routing.

---

# How Switching Works

1. Frame arrives at the switch.
2. Switch reads the Source MAC Address.
3. Source MAC Address is stored in the MAC Address Table.
4. Switch checks the Destination MAC Address.
5. Frame is forwarded to the correct port.

---

# MAC Address Table

A Switch maintains a MAC Address Table to remember which device is connected to which port.

Example

| MAC Address | Port |
|-------------|------|
|00:11:22:33:44:55|Fa0/1|
|00:AA:BB:CC:DD:EE|Fa0/2|

Cisco Command

```bash
show mac address-table
```

---

# Types of Switching

## 1. Store-and-Forward Switching

The switch receives the complete frame before forwarding it.

### Advantages

- Error Checking
- High Reliability
- Better Security

### Disadvantages

- Slightly Slower

---

## 2. Cut-Through Switching

The switch starts forwarding the frame as soon as it reads the destination MAC address.

### Advantages

- Very Fast
- Low Latency

### Disadvantages

- No Error Checking

---

## 3. Fragment-Free Switching

Reads the first 64 bytes before forwarding.

### Advantages

- Better than Cut-Through
- Detects Most Collision Errors

---

# Collision Domain

A Collision Domain is a network segment where packet collisions can occur.

Example

```
Hub → One Collision Domain
```

```
Switch → One Collision Domain per Port
```

---

# Broadcast Domain

A Broadcast Domain is the area where broadcast traffic is forwarded.

By default

```
One Switch = One Broadcast Domain
```

Using VLAN

```
Each VLAN = Separate Broadcast Domain
```

---

# Switching Methods Comparison

| Method | Speed | Error Checking |
|----------|-------|----------------|
| Store-and-Forward | Medium | Yes |
| Cut-Through | Fast | No |
| Fragment-Free | Fast | Partial |

---

# Managed vs Unmanaged Switch

| Managed Switch | Unmanaged Switch |
|----------------|------------------|
| Configurable | Plug and Play |
| Supports VLAN | No VLAN |
| Supports Security | Basic Features |
| Enterprise Networks | Home Networks |

---

# Cisco Switch Commands

Display MAC Address Table

```bash
show mac address-table
```

Display Running Configuration

```bash
show running-config
```

Display VLAN Information

```bash
show vlan brief
```

Display Interface Status

```bash
show interfaces status
```

Display Interface Configuration

```bash
show interfaces
```

Save Configuration

```bash
copy running-config startup-config
```

---

# Advantages

- High Speed
- Intelligent Forwarding
- Reduces Collisions
- Better Security
- Supports VLAN

---

# Disadvantages

- Higher Cost than Hub
- Requires Configuration
- Managed Switches Need Administration

---

# Real-Life Example

Imagine a courier office.

- Hub → Every parcel is sent to every house.
- Switch → Parcel is delivered only to the correct address.

---

# Interview Questions

1. What is Switching?
2. Which OSI Layer does a Switch operate on?
3. What is a MAC Address Table?
4. Difference between Hub and Switch?
5. What is Store-and-Forward Switching?
6. What is Cut-Through Switching?
7. What is Fragment-Free Switching?
8. What is a Collision Domain?
9. What is a Broadcast Domain?
10. Which Cisco command displays the MAC Address Table?

---

# Summary

Topics Covered

- Switching
- Switch
- MAC Address Table
- Store-and-Forward
- Cut-Through
- Fragment-Free
- Collision Domain
- Broadcast Domain
- Managed Switch
- Unmanaged Switch

Cisco Commands

- show mac address-table
- show running-config
- show vlan brief
- show interfaces
- copy running-config startup-config

**End of File**
