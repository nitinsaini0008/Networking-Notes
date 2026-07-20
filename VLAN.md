# VLAN (Virtual Local Area Network)

## About

A VLAN (Virtual Local Area Network) is a logical grouping of devices within a physical network. VLANs improve network performance, enhance security, and reduce broadcast traffic.

---

# What is VLAN?

A VLAN divides a single physical switch into multiple logical networks.

Example

```
Switch

├── VLAN 10 → HR Department
├── VLAN 20 → Sales Department
└── VLAN 30 → IT Department
```

Devices in different VLANs cannot communicate directly unless Inter-VLAN Routing is configured.

---

# Why Use VLAN?

- Reduces Broadcast Traffic
- Improves Security
- Better Network Performance
- Easy Network Management
- Logical Segmentation

---

# VLAN Types

## Default VLAN

- VLAN ID: 1
- Present on every Cisco switch.

---

## Data VLAN

Used for normal user data traffic.

Example

```
VLAN 10
```

---

## Management VLAN

Used to manage switches remotely.

Example

```
VLAN 99
```

---

## Native VLAN

Used on Trunk Ports for untagged traffic.

Default

```
VLAN 1
```

---

## Voice VLAN

Used for IP Phones.

Example

```
VLAN 100
```

---

# VLAN ID Range

| VLAN Range | Description |
|------------|-------------|
| 1 | Default VLAN |
| 2 – 1001 | Normal Range |
| 1002 – 1005 | Reserved |
| 1006 – 4094 | Extended Range |

---

# Access Port

An Access Port belongs to only one VLAN.

Example

```
PC → Switch (Access Port)
```

Cisco Command

```bash
switchport mode access
switchport access vlan 10
```

---

# Trunk Port

A Trunk Port carries traffic from multiple VLANs.

Example

```
Switch ←→ Switch
```

or

```
Switch ←→ Router
```

Cisco Command

```bash
switchport mode trunk
```

---

# VLAN Tagging

IEEE Standard

```
802.1Q
```

Adds VLAN information to Ethernet Frames.

---

# Inter-VLAN Routing

Allows communication between different VLANs using a Router or Layer 3 Switch.

Example

```
VLAN 10

↓

Router

↓

VLAN 20
```

---

# VLAN Configuration (Cisco)

Create VLAN

```bash
enable

configure terminal

vlan 10

name HR
```

Create Another VLAN

```bash
vlan 20

name SALES
```

Assign Port to VLAN

```bash
interface fastEthernet 0/1

switchport mode access

switchport access vlan 10
```

Configure Trunk Port

```bash
interface gigabitEthernet 0/1

switchport mode trunk
```

Save Configuration

```bash
copy running-config startup-config
```

---

# Verification Commands

Display VLANs

```bash
show vlan brief
```

Display Trunk Information

```bash
show interfaces trunk
```

Display Running Configuration

```bash
show running-config
```

Display Interface Status

```bash
show interfaces status
```

---

# Advantages

- Better Security
- Reduced Broadcast Domains
- Easy Administration
- Better Performance
- Efficient Network Utilization

---

# Disadvantages

- Initial Configuration Required
- Inter-VLAN Communication Requires Router or Layer 3 Switch
- Incorrect Configuration May Cause Connectivity Issues

---

# Real-Life Example

Imagine a company building.

- HR Department → VLAN 10
- Sales Department → VLAN 20
- IT Department → VLAN 30

Although everyone is inside the same building (same switch), each department works in its own separate network.

---

# Interview Questions

1. What is VLAN?
2. Why is VLAN used?
3. What is the difference between Access Port and Trunk Port?
4. What is Native VLAN?
5. What is Inter-VLAN Routing?
6. Which IEEE standard is used for VLAN tagging?
7. What is the default VLAN in Cisco switches?
8. Which command displays VLAN information?
9. Which command configures a trunk port?
10. Can two different VLANs communicate without a router?

---

# Summary

Topics Covered

- VLAN
- VLAN Types
- Access Port
- Trunk Port
- Native VLAN
- Voice VLAN
- VLAN Tagging
- Inter-VLAN Routing
- VLAN Configuration
- Verification Commands

Cisco Commands

- vlan
- name
- switchport mode access
- switchport access vlan
- switchport mode trunk
- show vlan brief
- show interfaces trunk
- copy running-config startup-config

**End of File**
