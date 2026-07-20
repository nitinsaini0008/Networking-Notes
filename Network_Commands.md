# Network Commands

## About

Network commands are utilities used to configure, monitor, troubleshoot, and test network connectivity. These commands are available on Windows, Linux, and macOS (some commands may differ).

---

# 1. ping

## Purpose

Tests connectivity between two devices.

## Syntax

```bash
ping <IP Address or Domain>
```

## Example

```bash
ping google.com
```

## Uses

- Check Network Connectivity
- Measure Response Time
- Verify Host Availability

---

# 2. ipconfig (Windows)

## Purpose

Displays and manages IP configuration.

## Syntax

```cmd
ipconfig
```

Useful Commands

Display Detailed Information

```cmd
ipconfig /all
```

Release IP Address

```cmd
ipconfig /release
```

Renew IP Address

```cmd
ipconfig /renew
```

Flush DNS Cache

```cmd
ipconfig /flushdns
```

Display DNS Cache

```cmd
ipconfig /displaydns
```

---

# 3. ifconfig (Linux - Legacy)

## Purpose

Displays or configures network interfaces.

## Syntax

```bash
ifconfig
```

Example

```bash
ifconfig eth0
```

> Note: On modern Linux distributions, the `ip` command is preferred.

---

# 4. ip Command (Linux)

## Purpose

Modern replacement for ifconfig.

## Show IP Address

```bash
ip addr
```

Show Interfaces

```bash
ip link
```

Show Routing Table

```bash
ip route
```

Bring Interface Up

```bash
sudo ip link set eth0 up
```

Bring Interface Down

```bash
sudo ip link set eth0 down
```

---

# 5. traceroute / tracert

## Purpose

Displays the path packets take to reach the destination.

### Linux

```bash
traceroute google.com
```

### Windows

```cmd
tracert google.com
```

---

# 6. netstat

## Purpose

Displays active network connections and listening ports.

## Syntax

```bash
netstat
```

Show Listening Ports

```bash
netstat -tuln
```

Windows

```cmd
netstat -ano
```

---

# 7. ss (Linux)

## Purpose

Modern replacement for netstat.

Show Listening Ports

```bash
ss -tuln
```

Show Active Connections

```bash
ss -tunap
```

---

# 8. arp

## Purpose

Displays or modifies the ARP cache.

## Windows

```cmd
arp -a
```

## Linux

```bash
arp -a
```

or

```bash
ip neigh
```

---

# 9. nslookup

## Purpose

Queries DNS servers to resolve domain names.

## Syntax

```bash
nslookup google.com
```

---

# 10. dig (Linux)

## Purpose

Provides detailed DNS information.

## Syntax

```bash
dig google.com
```

---

# 11. host (Linux)

## Purpose

Performs DNS lookups.

## Syntax

```bash
host google.com
```

---

# 12. curl

## Purpose

Transfers data from or to a server.

## View Webpage

```bash
curl https://example.com
```

View Headers Only

```bash
curl -I https://example.com
```

---

# 13. wget

## Purpose

Downloads files from the Internet.

## Syntax

```bash
wget https://example.com/file.zip
```

---

# 14. tcpdump (Linux)

## Purpose

Captures and analyzes network packets.

## Capture on All Interfaces

```bash
sudo tcpdump
```

Capture on Specific Interface

```bash
sudo tcpdump -i eth0
```

---

# 15. route

## Purpose

Displays the routing table.

### Windows

```cmd
route print
```

### Linux

```bash
ip route
```

---

# 16. hostname

## Purpose

Displays the computer's hostname.

```bash
hostname
```

---

# 17. whois

## Purpose

Displays domain registration information.

```bash
whois google.com
```

---

# 18. nmap

## Purpose

Scans hosts, ports, and services.

## Scan Host

```bash
nmap 192.168.1.1
```

Scan Open Ports

```bash
nmap google.com
```

---

# Common Commands Summary

| Command | Purpose |
|----------|---------|
| ping | Test Connectivity |
| ipconfig | Windows Network Configuration |
| ifconfig | Legacy Linux Network Configuration |
| ip | Linux Network Configuration |
| traceroute / tracert | Trace Packet Path |
| netstat | Display Network Connections |
| ss | Display Socket Information |
| arp | View ARP Cache |
| nslookup | DNS Lookup |
| dig | Detailed DNS Query |
| host | DNS Lookup |
| curl | Transfer Data |
| wget | Download Files |
| tcpdump | Packet Capture |
| route | Display Routing Table |
| hostname | Show Host Name |
| whois | Domain Information |
| nmap | Network Scanning |

---

# Advantages

- Easy Network Troubleshooting
- Helps Identify Connectivity Issues
- Useful for DNS Testing
- Monitors Network Traffic
- Essential for System and Network Administrators

---

# Real-Life Example

Suppose you cannot open a website.

You can troubleshoot using:

1. `ping` → Check connectivity.
2. `nslookup` → Verify DNS resolution.
3. `traceroute` → Find where packets stop.
4. `curl` → Test the web server response.
5. `tcpdump` → Capture and analyze packets.
6. `netstat` or `ss` → Check active connections.

---

# Interview Questions

1. What is the purpose of the `ping` command?
2. What is the difference between `ipconfig` and `ifconfig`?
3. Which command displays the routing table in Linux?
4. Which command flushes the DNS cache in Windows?
5. What is the purpose of `traceroute`?
6. Which command displays active network connections?
7. What is the difference between `netstat` and `ss`?
8. Which command captures network packets?
9. What is `nmap` used for?
10. Which command performs a DNS lookup?

---

# Summary

Topics Covered

- ping
- ipconfig
- ifconfig
- ip
- traceroute / tracert
- netstat
- ss
- arp
- nslookup
- dig
- host
- curl
- wget
- tcpdump
- route
- hostname
- whois
- nmap

These commands are essential for network administration, troubleshooting, cybersecurity, RHCSA, CCNA, and Linux system management.

**End of File**
