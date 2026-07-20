# OSI Model

## About

The OSI (Open Systems Interconnection) Model is a conceptual framework developed by the International Organization for Standardization (ISO). It explains how data travels from one computer to another over a network using seven different layers.

---

# What is the OSI Model?

The OSI Model divides network communication into **7 layers**. Each layer performs a specific task and communicates with the layer above and below it.

---

# OSI Layers

| Layer No. | Layer Name | Main Function |
|------------|----------------|----------------------------|
| 7 | Application | User Interface |
| 6 | Presentation | Data Formatting & Encryption |
| 5 | Session | Session Management |
| 4 | Transport | Reliable Data Transfer |
| 3 | Network | Routing & IP Addressing |
| 2 | Data Link | MAC Addressing |
| 1 | Physical | Transmission of Bits |

---

# Layer 7 – Application Layer

## Purpose

Provides network services directly to end users and applications.

## Protocols

- HTTP
- HTTPS
- FTP
- SMTP
- POP3
- IMAP
- DNS
- DHCP
- SSH
- Telnet

## Devices

- Computer
- Mobile
- Web Browser

---

# Layer 6 – Presentation Layer

## Purpose

Responsible for data translation, encryption, and compression.

## Functions

- Encryption
- Decryption
- Compression
- Data Formatting

## Examples

- SSL
- TLS
- JPEG
- PNG
- GIF
- MP3
- MPEG

---

# Layer 5 – Session Layer

## Purpose

Creates, manages, and terminates communication sessions.

## Functions

- Session Establishment
- Authentication
- Synchronization
- Session Termination

---

# Layer 4 – Transport Layer

## Purpose

Provides reliable data delivery.

## Protocols

- TCP
- UDP

## Functions

- Error Detection
- Flow Control
- Segmentation
- Reassembly

## Device

- Firewall

---

# Layer 3 – Network Layer

## Purpose

Determines the best path for data transmission.

## Protocols

- IPv4
- IPv6
- ICMP
- OSPF
- RIP
- EIGRP

## Device

- Router

---

# Layer 2 – Data Link Layer

## Purpose

Provides node-to-node communication.

## Functions

- MAC Address
- Error Detection
- Frame Delivery

## Protocols

- Ethernet
- PPP
- HDLC

## Device

- Switch
- Bridge

---

# Layer 1 – Physical Layer

## Purpose

Transmits raw binary data through cables and wireless media.

## Media

- UTP Cable
- Fiber Optic
- Coaxial Cable
- Wireless

## Devices

- Hub
- Repeater

---

# Data Encapsulation

| Layer | Data Unit |
|---------|-----------|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

---

# Memory Trick

```
All
People
Seem
To
Need
Data
Processing
```

Bottom to Top

```
Please
Do
Not
Throw
Sausage
Pizza
Away
```

---

# Advantages

- Easy Troubleshooting
- Modular Design
- Standard Communication
- Easy Learning
- Vendor Independence

---

# Disadvantages

- Complex Model
- Mostly Theoretical
- Not Fully Implemented

---

# Real-Life Example

Imagine sending a parcel:

- Application → Write the letter
- Presentation → Pack the gift
- Session → Contact courier
- Transport → Courier service
- Network → Select route
- Data Link → Local delivery center
- Physical → Delivery vehicle

---

# Interview Questions

1. What is the OSI Model?
2. Who developed the OSI Model?
3. How many layers are in the OSI Model?
4. Which layer uses IP Address?
5. Which layer uses MAC Address?
6. Which layer is responsible for Routing?
7. Difference between Layer 2 and Layer 3?
8. Which protocols work on the Transport Layer?
9. Which device works on Layer 2?
10. Which device works on Layer 3?
11. Which layer is responsible for Encryption?
12. What is Encapsulation?

---

# Summary

Layers Covered

- Physical
- Data Link
- Network
- Transport
- Session
- Presentation
- Application

Devices Covered

- Hub
- Switch
- Router
- Firewall

Protocols Covered

- TCP
- UDP
- HTTP
- HTTPS
- FTP
- DNS
- DHCP
- SSH
- IPv4
- IPv6

**End of File**
