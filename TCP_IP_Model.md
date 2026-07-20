# TCP/IP Model

## About

The TCP/IP (Transmission Control Protocol/Internet Protocol) Model is the standard networking model used on the Internet. It defines how devices communicate, send, receive, and route data across networks.

---

# What is TCP/IP Model?

The TCP/IP Model consists of **4 layers**.

It was developed by the **United States Department of Defense (DoD)** and is the foundation of modern Internet communication.

---

# TCP/IP Layers

| Layer | Name | Function |
|--------|------|----------|
| 4 | Application | Provides network services to users |
| 3 | Transport | Reliable data transfer |
| 2 | Internet | Logical addressing & routing |
| 1 | Network Access | Physical transmission of data |

---

# 1. Application Layer

## Purpose

Provides services directly to user applications.

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

## Examples

- Chrome
- Firefox
- Outlook
- Gmail
- FileZilla

---

# 2. Transport Layer

## Purpose

Provides end-to-end communication.

## Protocols

### TCP

Features

- Reliable
- Connection-Oriented
- Error Checking
- Flow Control
- Acknowledgement

Examples

- HTTP
- HTTPS
- FTP
- SSH

---

### UDP

Features

- Faster
- Connectionless
- No Acknowledgement
- Low Overhead

Examples

- DNS
- VoIP
- Live Streaming
- Online Gaming

---

# TCP vs UDP

| TCP | UDP |
|------|-----|
| Reliable | Fast |
| Connection-Oriented | Connectionless |
| Error Checking | No Error Recovery |
| Slower | Faster |
| Large Header | Small Header |

---

# 3. Internet Layer

## Purpose

Responsible for routing packets between networks.

## Protocols

- IPv4
- IPv6
- ICMP
- ARP

## Device

- Router

---

# 4. Network Access Layer

## Purpose

Handles physical transmission of data.

## Technologies

- Ethernet
- Wi-Fi
- Fiber
- UTP Cable

## Devices

- Switch
- Hub
- NIC

---

# Data Units

| Layer | Data Unit |
|---------|-----------|
| Application | Data |
| Transport | Segment |
| Internet | Packet |
| Network Access | Frame/Bits |

---

# TCP Three-Way Handshake

## Step 1

Client → SYN

## Step 2

Server → SYN + ACK

## Step 3

Client → ACK

Connection Established

---

# TCP Connection Termination

1. FIN
2. ACK
3. FIN
4. ACK

---

# Port Numbers

| Protocol | Port |
|-----------|------|
| HTTP | 80 |
| HTTPS | 443 |
| FTP | 21 |
| SSH | 22 |
| Telnet | 23 |
| SMTP | 25 |
| DNS | 53 |
| DHCP | 67 / 68 |
| POP3 | 110 |
| IMAP | 143 |

---

# OSI vs TCP/IP

| OSI Model | TCP/IP Model |
|------------|--------------|
| 7 Layers | 4 Layers |
| Theoretical | Practical |
| ISO | DoD |
| Rarely Implemented | Used Worldwide |

---

# Advantages

- Standard Internet Model
- Highly Scalable
- Reliable Communication
- Supports Multiple Networks
- Platform Independent

---

# Disadvantages

- Complex Configuration
- Security Not Built-in
- Protocol Overhead

---

# Real-Life Example

Sending a WhatsApp message:

Application Layer → WhatsApp

Transport Layer → TCP delivers data reliably.

Internet Layer → IP finds the destination.

Network Access Layer → Wi-Fi/Ethernet sends the data.

---

# Interview Questions

1. What is TCP/IP?
2. How many layers are in the TCP/IP model?
3. Difference between TCP and UDP?
4. What is a Three-Way Handshake?
5. What is the Internet Layer?
6. Which protocol uses Port 80?
7. Which protocol uses Port 443?
8. What is the difference between OSI and TCP/IP?
9. Which protocol is used for secure remote login?
10. Which protocol is faster, TCP or UDP?

---

# Summary

Layers Covered

- Application
- Transport
- Internet
- Network Access

Protocols Covered

- TCP
- UDP
- IPv4
- IPv6
- HTTP
- HTTPS
- FTP
- SSH
- DNS
- DHCP

Topics Covered

- TCP vs UDP
- Three-Way Handshake
- Port Numbers
- OSI vs TCP/IP

**End of File**
