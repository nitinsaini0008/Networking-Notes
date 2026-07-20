# Networking Interview Questions & Answers

## About

This document contains important networking interview questions with short and easy-to-understand answers. These questions are useful for:

- CCNA Preparation
- RHCSA Interviews
- Cyber Security Interviews
- Network Support Engineer
- System Administrator
- Technical Support Engineer
- Campus Placements

---

# Basic Networking Questions

## 1. What is a Computer Network?

A Computer Network is a group of interconnected devices that communicate and share resources.

---

## 2. What is an IP Address?

An IP Address is a unique logical address assigned to a device for communication on a network.

---

## 3. What is a MAC Address?

A MAC Address is a unique physical address assigned to a Network Interface Card (NIC).

---

## 4. Difference between IP Address and MAC Address?

| IP Address | MAC Address |
|------------|-------------|
| Logical Address | Physical Address |
| Can Change | Permanent |
| Layer 3 | Layer 2 |

---

## 5. What is a Router?

A Router connects different networks and forwards packets using IP addresses.

---

## 6. What is a Switch?

A Switch connects devices in a LAN using MAC addresses.

---

## 7. What is a Hub?

A Hub broadcasts incoming data to all connected devices.

---

## 8. What is DNS?

DNS converts domain names into IP addresses.

---

## 9. What is DHCP?

DHCP automatically assigns IP addresses to network devices.

---

## 10. What is Gateway?

A Gateway is the device that connects a local network to another network, such as the Internet.

---

# OSI Model Questions

## 11. How many layers are in the OSI Model?

7 Layers.

---

## 12. Name the OSI Layers.

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

---

## 13. Which layer uses IP Address?

Network Layer.

---

## 14. Which layer uses MAC Address?

Data Link Layer.

---

## 15. Which OSI layer does a Router work on?

Layer 3.

---

## 16. Which OSI layer does a Switch work on?

Layer 2.

---

## 17. Which OSI layer does a Hub work on?

Layer 1.

---

## 18. Which protocol works at the Transport Layer?

TCP and UDP.

---

## 19. What is Encapsulation?

The process of adding protocol headers to data before transmission.

---

## 20. What is Decapsulation?

The process of removing protocol headers at the receiving end.

---

# TCP/IP Questions

## 21. Difference between TCP and UDP?

| TCP | UDP |
|------|-----|
| Reliable | Unreliable |
| Connection-Oriented | Connectionless |
| Slower | Faster |

---

## 22. What is the TCP Three-Way Handshake?

SYN → SYN-ACK → ACK.

---

## 23. What is a Port Number?

A logical communication endpoint used by applications.

---

## 24. What is the HTTP Port?

80.

---

## 25. What is the HTTPS Port?

443.

---

## 26. What is the FTP Port?

21.

---

## 27. What is the SSH Port?

22.

---

## 28. What is the Telnet Port?

23.

---

## 29. What is the DNS Port?

53.

---

## 30. What is the DHCP Port?

UDP 67 and UDP 68.

---

# Routing & Switching

## 31. What is Routing?

Selecting the best path to send packets between networks.

---

## 32. What is Static Routing?

Routes configured manually.

---

## 33. What is Dynamic Routing?

Routes learned automatically using routing protocols.

---

## 34. Name Dynamic Routing Protocols.

- RIP
- OSPF
- EIGRP

---

## 35. What is VLAN?

A logical separation of a physical network.

---

## 36. What is Inter-VLAN Routing?

Communication between different VLANs using a Router or Layer 3 Switch.

---

## 37. What is a Trunk Port?

Carries traffic from multiple VLANs.

---

## 38. What is an Access Port?

Belongs to only one VLAN.

---

## 39. What is a Collision Domain?

A network segment where packet collisions can occur.

---

## 40. What is a Broadcast Domain?

A group of devices that receive broadcast traffic.

---

# Security Questions

## 41. What is a Firewall?

A security device that filters network traffic.

---

## 42. What is ACL?

Access Control List used to allow or deny traffic.

---

## 43. What is NAT?

Network Address Translation converts private IPs into public IPs.

---

## 44. What is PAT?

Port Address Translation allows multiple devices to share one public IP.

---

## 45. Why is SSH preferred over Telnet?

SSH encrypts communication while Telnet sends data in plain text.

---

## 46. What is HTTPS?

The secure version of HTTP using SSL/TLS encryption.

---

## 47. What is SSL/TLS?

Protocols used to encrypt network communication.

---

## 48. What is Wireshark?

A packet capture and protocol analysis tool.

---

## 49. What is Packet Sniffing?

Capturing and analyzing network traffic.

---

## 50. What is VPN?

A Virtual Private Network that provides secure communication over the Internet.

---

# Linux & Troubleshooting

## 51. Which command checks connectivity?

```bash
ping
```

---

## 52. Which command displays the routing table?

```bash
ip route
```

---

## 53. Which command shows IP addresses in Linux?

```bash
ip addr
```

---

## 54. Which command shows IP configuration in Windows?

```cmd
ipconfig /all
```

---

## 55. Which command checks DNS?

```bash
nslookup google.com
```

---

## 56. Which command captures packets?

```bash
tcpdump
```

---

## 57. Which command displays open ports?

```bash
ss -tuln
```

or

```bash
netstat -tuln
```

---

## 58. Which command traces packet routes?

```bash
traceroute
```

or

```cmd
tracert
```

---

## 59. Which command scans hosts?

```bash
nmap
```

---

## 60. Which command displays the ARP cache?

```bash
arp -a
```

---

# Cisco Questions

## 61. Which command enters privileged mode?

```bash
enable
```

---

## 62. Which command enters global configuration mode?

```bash
configure terminal
```

---

## 63. Which command displays the running configuration?

```bash
show running-config
```

---

## 64. Which command saves the configuration?

```bash
copy running-config startup-config
```

---

## 65. Which command displays VLANs?

```bash
show vlan brief
```

---

## 66. Which command displays the routing table?

```bash
show ip route
```

---

## 67. Which command displays interfaces?

```bash
show ip interface brief
```

---

## 68. Which command displays the MAC table?

```bash
show mac address-table
```

---

## 69. Which command configures an Access Port?

```bash
switchport mode access
```

---

## 70. Which command configures a Trunk Port?

```bash
switchport mode trunk
```

---

# Rapid Fire Questions

71. IPv4 Address Size? → **32 Bits**

72. IPv6 Address Size? → **128 Bits**

73. Loopback Address? → **127.0.0.1**

74. APIPA Range? → **169.254.0.0/16**

75. Private Class A? → **10.0.0.0/8**

76. Private Class B? → **172.16.0.0 – 172.31.255.255**

77. Private Class C? → **192.168.0.0/16**

78. Broadcast Address? → **255.255.255.255**

79. Default Gateway Purpose? → **Connects to Other Networks**

80. DNS Full Form? → **Domain Name System**

81. DHCP Full Form? → **Dynamic Host Configuration Protocol**

82. NAT Full Form? → **Network Address Translation**

83. VLAN Full Form? → **Virtual Local Area Network**

84. FTP Full Form? → **File Transfer Protocol**

85. SSH Full Form? → **Secure Shell**

86. HTTP Full Form? → **HyperText Transfer Protocol**

87. HTTPS Full Form? → **HyperText Transfer Protocol Secure**

88. TCP Full Form? → **Transmission Control Protocol**

89. UDP Full Form? → **User Datagram Protocol**

90. ICMP Full Form? → **Internet Control Message Protocol**

91. ARP Full Form? → **Address Resolution Protocol**

92. MAC Full Form? → **Media Access Control**

93. LAN Full Form? → **Local Area Network**

94. WAN Full Form? → **Wide Area Network**

95. MAN Full Form? → **Metropolitan Area Network**

96. PAN Full Form? → **Personal Area Network**

97. ISP Full Form? → **Internet Service Provider**

98. NIC Full Form? → **Network Interface Card**

99. OSI Full Form? → **Open Systems Interconnection**

100. TCP is Reliable? → **Yes**

---

# Summary

This document includes **100 important networking interview questions and answers** covering:

- Basic Networking
- OSI Model
- TCP/IP
- Routing & Switching
- VLAN
- DHCP
- DNS
- NAT
- HTTP/HTTPS
- SSH
- Telnet
- Firewalls
- Wireshark
- Linux Networking
- Cisco CLI
- Rapid-Fire Interview Questions

These questions are ideal for **CCNA, RHCSA, Cyber Security, Network Engineer, Technical Support, and Campus Placement interviews**.

**End of File**
