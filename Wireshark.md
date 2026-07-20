# Wireshark

## About

Wireshark is a free and open-source network protocol analyzer used to capture and inspect network packets in real time. It helps network administrators, cybersecurity professionals, and students analyze network traffic, troubleshoot problems, and understand how protocols work.

---

# What is Wireshark?

Wireshark captures packets traveling across a network and displays detailed information about each packet.

Example

```
Computer

↓

Network Traffic

↓

Wireshark

↓

Packet Analysis
```

---

# Why Use Wireshark?

- Capture Network Packets
- Analyze Network Traffic
- Troubleshoot Network Problems
- Detect Security Issues
- Learn Networking Protocols

---

# Features

- Live Packet Capture
- Deep Packet Inspection
- Protocol Analysis
- Packet Filtering
- Export Captured Packets
- Supports Thousands of Protocols

---

# Packet Capture Process

1. Select a Network Interface.
2. Start Packet Capture.
3. Generate Network Traffic.
4. Stop Packet Capture.
5. Analyze Captured Packets.

---

# Packet Structure

Each packet contains:

- Frame Information
- Ethernet Header
- IP Header
- TCP/UDP Header
- Application Data

---

# Packet Details

## Frame

Contains packet length, arrival time, and frame number.

---

## Ethernet Header

Contains:

- Source MAC Address
- Destination MAC Address

---

## IP Header

Contains:

- Source IP Address
- Destination IP Address
- TTL
- Protocol

---

## TCP Header

Contains:

- Source Port
- Destination Port
- Sequence Number
- Acknowledgment Number
- Flags

---

## Application Data

Contains protocol-specific information such as:

- HTTP
- DNS
- FTP
- SSH

---

# TCP Three-Way Handshake

Connection establishment uses three steps.

```
Client

↓

SYN

↓

Server

↓

SYN-ACK

↓

Client

↓

ACK

↓

Connection Established
```

---

# Common Protocols in Wireshark

| Protocol | Purpose |
|----------|---------|
| ARP | Address Resolution |
| ICMP | Ping |
| TCP | Reliable Communication |
| UDP | Fast Communication |
| HTTP | Web Browsing |
| HTTPS | Secure Web Browsing |
| DNS | Domain Name Resolution |
| DHCP | Automatic IP Assignment |
| FTP | File Transfer |
| SSH | Secure Remote Access |

---

# Display Filters

Display Filters show only matching packets.

HTTP Traffic

```text
http
```

HTTPS Traffic

```text
tls
```

DNS Packets

```text
dns
```

TCP Packets

```text
tcp
```

UDP Packets

```text
udp
```

ICMP (Ping)

```text
icmp
```

ARP

```text
arp
```

FTP

```text
ftp
```

SSH

```text
ssh
```

Specific IP Address

```text
ip.addr == 192.168.1.10
```

Source IP

```text
ip.src == 192.168.1.10
```

Destination IP

```text
ip.dst == 192.168.1.20
```

Specific TCP Port

```text
tcp.port == 80
```

HTTP GET Requests

```text
http.request.method == "GET"
```

---

# Capture Filters

Capture Filters limit packets before capture begins.

Capture Only HTTP

```text
tcp port 80
```

Capture HTTPS

```text
tcp port 443
```

Capture DNS

```text
port 53
```

Capture SSH

```text
port 22
```

Capture ICMP

```text
icmp
```

---

# Useful Wireshark Options

Find Packet

```
Ctrl + F
```

Follow TCP Stream

```
Right Click

↓

Follow

↓

TCP Stream
```

Export Packets

```
File

↓

Export Specified Packets
```

---

# Common Troubleshooting Tasks

- Identify Packet Loss
- Detect High Network Latency
- Analyze TCP Handshakes
- Verify DNS Resolution
- Inspect HTTP Requests
- Check TLS Handshakes
- Troubleshoot DHCP Issues
- Detect Duplicate IP Addresses

---

# Advantages

- Free and Open Source
- Supports Thousands of Protocols
- Excellent Troubleshooting Tool
- Detailed Packet Analysis
- Cross-Platform Support

---

# Disadvantages

- Large Captures Can Be Difficult to Analyze
- Requires Networking Knowledge
- High Memory Usage During Large Captures

---

# Real-Life Example

Imagine CCTV cameras recording everything happening inside a building.

Later, security personnel review the footage to find what happened.

Similarly,

Wireshark records network traffic so administrators can analyze communication between devices.

---

# Interview Questions

1. What is Wireshark?
2. Why is Wireshark used?
3. What is the difference between Capture Filters and Display Filters?
4. Explain the TCP Three-Way Handshake.
5. Which filter displays only DNS packets?
6. Which protocol is used for Ping?
7. Which filter displays traffic for a specific IP address?
8. How do you follow a TCP conversation in Wireshark?
9. Can Wireshark decrypt HTTPS traffic by default?
10. Name five protocols supported by Wireshark.

---

# Summary

Topics Covered

- Wireshark
- Packet Capture
- Packet Structure
- TCP Three-Way Handshake
- Protocol Analysis
- Display Filters
- Capture Filters
- Packet Inspection
- Troubleshooting
- Interview Questions

Common Filters

- http
- dns
- tcp
- udp
- icmp
- arp
- ftp
- ssh
- ip.addr
- tcp.port

**End of File**
