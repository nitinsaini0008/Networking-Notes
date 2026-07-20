# Telnet

## About

Telnet is an application-layer protocol used to remotely access and manage computers or network devices over a TCP/IP network. It provides a command-line interface (CLI) for remote administration but does not encrypt data, making it insecure for modern networks.

---

# What is Telnet?

Telnet allows users to remotely log in to another computer or network device.

Example

```
Your Computer

↓

Telnet Connection

↓

Router / Switch / Server
```

---

# Default Port

| Protocol | Port |
|----------|------|
| Telnet | 23 |

---

# Why was Telnet Used?

- Remote Device Management
- Server Administration
- Network Troubleshooting
- Remote Command Execution

Today, SSH is preferred because it provides secure encrypted communication.

---

# How Telnet Works

1. Client starts a Telnet session.
2. Client connects to the remote device on Port 23.
3. User enters username and password.
4. Authentication is performed.
5. User executes commands remotely.
6. Session ends after logout.

---

# Features

- Remote Command-Line Access
- Client-Server Architecture
- Simple Configuration
- Plain Text Communication
- Cross-Platform Support

---

# Telnet Communication

```
Client

↓

TCP Port 23

↓

Remote Device

↓

Command Execution
```

---

# Installing Telnet

## Windows

Enable Telnet Client

```
Control Panel

↓

Programs

↓

Turn Windows Features On or Off

↓

Telnet Client
```

---

## Linux (RHEL/CentOS)

Install Telnet Client

```bash
sudo yum install telnet
```

or

```bash
sudo dnf install telnet
```

---

## Ubuntu/Debian

```bash
sudo apt update

sudo apt install telnet
```

---

# Common Telnet Commands

Connect to a Device

```bash
telnet 192.168.1.10
```

Connect Using Hostname

```bash
telnet example.com
```

Connect to a Specific Port

```bash
telnet example.com 80
```

Exit Session

```text
quit
```

or

```text
exit
```

---

# Cisco Telnet Configuration

Enable Telnet Access

```bash
configure terminal
```

Configure VTY Lines

```bash
line vty 0 4
```

Set Password

```bash
password cisco
```

Enable Login

```bash
login
```

Allow Telnet

```bash
transport input telnet
```

Save Configuration

```bash
copy running-config startup-config
```

---

# Verify Configuration

Display Running Configuration

```bash
show running-config
```

Display Active Users

```bash
show users
```

Display Current Sessions

```bash
show line
```

---

# Security Risks

Telnet sends the following information in plain text:

- Username
- Password
- Commands
- Data

Anyone capturing network traffic can read this information.

---

# Telnet vs SSH

| Feature | Telnet | SSH |
|---------|--------|-----|
| Port | 23 | 22 |
| Encryption | No | Yes |
| Security | Low | High |
| Authentication | Plain Text | Encrypted |
| Remote Access | Yes | Yes |
| Recommended | No | Yes |

---

# Advantages

- Easy to Configure
- Lightweight Protocol
- Useful for Basic Connectivity Testing
- Supported on Many Devices

---

# Disadvantages

- No Encryption
- Passwords Sent in Plain Text
- Vulnerable to Packet Sniffing
- Not Recommended for Production Networks

---

# Real-Life Example

Imagine speaking to someone over a loudspeaker.

With Telnet:

```
Everyone nearby can hear your conversation.
```

With SSH:

```
The conversation happens in a private, soundproof room.
```

---

# Interview Questions

1. What is Telnet?
2. What is the default Telnet port?
3. Why is Telnet considered insecure?
4. What is the difference between Telnet and SSH?
5. Which protocol should be used instead of Telnet?
6. Which Cisco command enables Telnet access?
7. Which command configures VTY lines?
8. Which command shows active users?
9. Can Telnet encrypt data?
10. What are the disadvantages of Telnet?

---

# Summary

Topics Covered

- Telnet
- Telnet Working
- Port 23
- Cisco Telnet Configuration
- Telnet Commands
- Security Risks
- Telnet vs SSH
- Advantages
- Disadvantages

Common Port

- Telnet: 23

Common Commands

- telnet
- line vty 0 4
- password
- login
- transport input telnet
- show users
- show line

**End of File**
