# MAC Address

## About

A MAC (Media Access Control) Address is a unique physical address assigned to every Network Interface Card (NIC). It is used for communication within a Local Area Network (LAN).

---

# What is a MAC Address?

A MAC Address is a **48-bit (6-byte)** hardware address permanently assigned to a network device by the manufacturer.

Example

```text
00:1A:2B:3C:4D:5E
```

---

# MAC Address Format

A MAC Address consists of **6 groups**, each containing **2 hexadecimal digits**.

Example

```text
00:1A:2B:3C:4D:5E
```

Each hexadecimal digit ranges from:

```text
0-9
A-F
```

---

# Structure of MAC Address

Example

```text
00:1A:2B:3C:4D:5E
```

- First 24 bits → OUI (Organizationally Unique Identifier)
- Last 24 bits → Device Identifier

---

# Types of MAC Address

## 1. Unicast MAC

Used for communication between one sender and one receiver.

Example

```text
00:1A:2B:3C:4D:5E
```

---

## 2. Multicast MAC

Used to send data to multiple devices.

Example

```text
01:00:5E:XX:XX:XX
```

---

## 3. Broadcast MAC

Used to send data to every device in the LAN.

Address

```text
FF:FF:FF:FF:FF:FF
```

---

# MAC Address vs IP Address

| MAC Address | IP Address |
|-------------|------------|
| Physical Address | Logical Address |
| Layer 2 | Layer 3 |
| Permanent | Can Change |
| Used Inside LAN | Used Across Networks |
| 48-bit | IPv4 = 32-bit, IPv6 = 128-bit |

---

# MAC Address Table

Switches maintain a MAC Address Table to forward frames efficiently.

Example

| MAC Address | Port |
|-------------|------|
|00:1A:2B:3C:4D:5E|Fa0/1|
|08:11:22:33:44:55|Fa0/2|

---

# How to View MAC Address

## Windows

```cmd
ipconfig /all
```

---

## Linux

```bash
ip link
```

or

```bash
ifconfig
```

---

## Cisco Switch

```text
show mac address-table
```

---

# MAC Address Spoofing

MAC Address Spoofing is the process of changing the MAC Address of a device using software.

Uses

- Privacy Testing
- Security Testing
- Penetration Testing

---

# Advantages

- Unique Device Identification
- Fast Communication Inside LAN
- Helps Switches Forward Frames
- Required for Ethernet Communication

---

# Limitations

- Works Only in Local Network
- Cannot Route Between Networks
- Can Be Spoofed

---

# Real-Life Example

Imagine a housing society.

- IP Address = Flat Number
- MAC Address = Resident's Aadhaar Number

Even if the flat changes, the person's identity remains unique.

---

# Interview Questions

1. What is a MAC Address?
2. Which OSI Layer uses MAC Address?
3. How many bits are in a MAC Address?
4. Difference between MAC Address and IP Address?
5. What is Broadcast MAC Address?
6. What is OUI?
7. Which device stores the MAC Address Table?
8. What is MAC Address Spoofing?
9. Which command displays the MAC Address in Linux?
10. Which command displays the MAC Address Table in Cisco Switch?

---

# Summary

Topics Covered

- MAC Address
- OUI
- Unicast
- Multicast
- Broadcast
- MAC Table
- MAC vs IP
- MAC Spoofing
- Linux Commands
- Cisco Commands

**End of File**
