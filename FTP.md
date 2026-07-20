# FTP (File Transfer Protocol)

## About

File Transfer Protocol (FTP) is a standard network protocol used to transfer files between a client and a server over a TCP/IP network.

FTP allows users to upload, download, rename, delete, and manage files on a remote server.

---

# What is FTP?

FTP is one of the oldest Internet protocols used for file sharing.

Example

```
Your Computer (FTP Client)

↓

Internet

↓

FTP Server
```

The client connects to the FTP server to exchange files.

---

# Default Port Numbers

| Protocol | Port |
|----------|------|
| FTP Control Connection | 21 |
| FTP Data Connection | 20 |

---

# How FTP Works

1. Client connects to the FTP Server.
2. Authentication takes place using Username and Password.
3. Server verifies credentials.
4. Control connection is established.
5. Data connection is created.
6. Files are uploaded or downloaded.
7. Session ends.

---

# FTP Components

## FTP Client

Software used to connect to an FTP server.

Examples

- FileZilla
- WinSCP
- Cyberduck
- Command Line FTP

---

## FTP Server

Stores files and responds to FTP client requests.

Examples

- vsftpd (Linux)
- ProFTPD
- FileZilla Server
- Microsoft IIS FTP

---

# FTP Modes

## 1. Active Mode

In Active Mode:

- Client opens a random port.
- Server connects back to the client on Port 20.

Advantages

- Faster in some environments.

Disadvantages

- Often blocked by firewalls.

---

## 2. Passive Mode

In Passive Mode:

- Client requests a data connection.
- Server opens a random port.
- Client connects to that port.

Advantages

- Firewall Friendly
- Most Common Today

Disadvantages

- Slightly More Server Configuration

---

# Active vs Passive FTP

| Feature | Active | Passive |
|---------|---------|----------|
| Server Initiates Data Connection | Yes | No |
| Client Initiates Data Connection | No | Yes |
| Firewall Friendly | No | Yes |
| Common Today | No | Yes |

---

# Anonymous FTP

Anonymous FTP allows users to access files without creating a user account.

Typical Login

```
Username: anonymous

Password: user@example.com
```

Used for:

- Public Downloads
- Software Repositories
- Documentation

---

# Common FTP Commands

Connect to Server

```bash
ftp 192.168.1.10
```

Display Current Directory

```bash
pwd
```

List Files

```bash
ls
```

Change Directory

```bash
cd folder_name
```

Upload File

```bash
put file.txt
```

Download File

```bash
get file.txt
```

Download Multiple Files

```bash
mget *.txt
```

Upload Multiple Files

```bash
mput *.txt
```

Delete File

```bash
delete file.txt
```

Rename File

```bash
rename old.txt new.txt
```

Exit FTP

```bash
bye
```

or

```bash
quit
```

---

# FTP Security

Standard FTP does **not** encrypt:

- Username
- Password
- Data

Anyone monitoring the network can potentially capture this information.

---

# Secure Alternatives

## FTPS (FTP Secure)

- Uses SSL/TLS Encryption
- Secure version of FTP
- Default Port: 990 (Implicit FTPS)

---

## SFTP (SSH File Transfer Protocol)

- Uses SSH Protocol
- Fully Encrypted
- Default Port: 22

> Note: SFTP is **not** the same as FTP.

---

# FTP Configuration (Linux vsftpd)

Install

```bash
sudo yum install vsftpd
```

or

```bash
sudo dnf install vsftpd
```

Start Service

```bash
sudo systemctl start vsftpd
```

Enable Service

```bash
sudo systemctl enable vsftpd
```

Check Status

```bash
sudo systemctl status vsftpd
```

---

# Advantages

- Fast File Transfer
- Easy to Use
- Supports Large Files
- Widely Supported
- Cross-Platform

---

# Disadvantages

- No Encryption in Standard FTP
- Username and Password Sent in Plain Text
- Vulnerable to Packet Sniffing
- Firewall Configuration May Be Required

---

# Real-Life Example

Imagine a courier service.

- FTP Server → Warehouse
- FTP Client → Customer
- Upload → Sending a Parcel
- Download → Receiving a Parcel

---

# Interview Questions

1. What is FTP?
2. What is the default FTP port?
3. What is the difference between Active and Passive FTP?
4. Why is standard FTP considered insecure?
5. What is Anonymous FTP?
6. What is the difference between FTP, FTPS, and SFTP?
7. Which port does SFTP use?
8. Which Linux package is commonly used as an FTP server?
9. Which command uploads a file?
10. Which command lists files on the FTP server?

---

# Summary

Topics Covered

- FTP
- FTP Client
- FTP Server
- Active Mode
- Passive Mode
- Anonymous FTP
- FTP Commands
- FTPS
- SFTP
- vsftpd Configuration

Common Ports

- FTP: 21
- FTP Data: 20
- FTPS: 990
- SFTP: 22

**End of File**
