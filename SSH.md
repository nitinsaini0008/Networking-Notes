# SSH (Secure Shell)

## About

Secure Shell (SSH) is a secure network protocol used to remotely access and manage computers and servers over an unsecured network. SSH encrypts all communication between the client and the server, making it much more secure than Telnet.

---

# What is SSH?

SSH allows administrators and users to securely log in to remote systems, execute commands, transfer files, and manage servers.

Example

```
Your Computer

↓

SSH Connection

↓

Remote Linux Server
```

---

# Default Port

| Protocol | Port |
|----------|------|
| SSH | 22 |

---

# Why Use SSH?

- Secure Remote Login
- Encrypted Communication
- File Transfer Support
- Remote Administration
- Secure Command Execution

---

# How SSH Works

1. Client requests connection.
2. Server sends its public key.
3. Client verifies the server.
4. User authenticates.
5. Secure encrypted session begins.

---

# SSH Authentication Methods

## 1. Password Authentication

User enters:

- Username
- Password

Example

```bash
ssh user@192.168.1.10
```

---

## 2. Public Key Authentication

Uses a pair of cryptographic keys.

- Private Key (Stored on Client)
- Public Key (Stored on Server)

More secure than passwords.

---

# Generate SSH Key Pair

Generate RSA Key

```bash
ssh-keygen -t rsa
```

Generate ED25519 Key (Recommended)

```bash
ssh-keygen -t ed25519
```

Default Key Location

```
~/.ssh/
```

Files Created

```
id_rsa

id_rsa.pub
```

or

```
id_ed25519

id_ed25519.pub
```

---

# Copy Public Key to Server

```bash
ssh-copy-id user@192.168.1.10
```

Now login without entering the password.

---

# Common SSH Commands

Connect to Remote Server

```bash
ssh user@192.168.1.10
```

Connect Using Different Port

```bash
ssh -p 2222 user@192.168.1.10
```

Display SSH Version

```bash
ssh -V
```

Exit SSH Session

```bash
exit
```

---

# SCP (Secure Copy Protocol)

Used to securely transfer files over SSH.

Copy Local File to Remote Server

```bash
scp file.txt user@192.168.1.10:/home/user/
```

Copy Remote File to Local Computer

```bash
scp user@192.168.1.10:/home/user/file.txt .
```

---

# SFTP (SSH File Transfer Protocol)

Provides secure file transfer using SSH.

Start SFTP Session

```bash
sftp user@192.168.1.10
```

Useful Commands

```bash
ls
pwd
cd
put file.txt
get file.txt
exit
```

---

# SSH Configuration File

Configuration File

```
/etc/ssh/sshd_config
```

Common Settings

Change SSH Port

```text
Port 22
```

Disable Root Login

```text
PermitRootLogin no
```

Disable Password Authentication

```text
PasswordAuthentication no
```

Allow Specific Users

```text
AllowUsers admin nitin
```

Restart SSH Service

```bash
sudo systemctl restart sshd
```

or

```bash
sudo systemctl restart ssh
```

---

# Verify SSH Service

Check Status

```bash
systemctl status sshd
```

Check Listening Port

```bash
ss -tuln | grep 22
```

or

```bash
netstat -tuln | grep 22
```

---

# SSH Security Best Practices

- Use SSH Keys Instead of Passwords
- Disable Root Login
- Change Default Port (Optional)
- Keep SSH Updated
- Use Strong Passphrases
- Enable Firewall Rules
- Disable Unused Accounts
- Limit Login Attempts

---

# Advantages

- Strong Encryption
- Secure Remote Access
- Secure File Transfer
- Cross-Platform Support
- Supports Key-Based Authentication

---

# Disadvantages

- Initial Configuration Required
- Key Management Can Be Complex
- Brute Force Attacks Possible if Misconfigured

---

# SSH vs Telnet

| Feature | SSH | Telnet |
|---------|-----|--------|
|Port|22|23|
|Encryption|Yes|No|
|Authentication|Secure|Plain Text|
|Security|High|Low|
|Recommended|Yes|No|

---

# Real-Life Example

Imagine visiting a bank locker.

Without SSH

```
Anyone can hear your conversation.
```

With SSH

```
You enter a secure private room where nobody else can listen.
```

---

# Interview Questions

1. What is SSH?
2. What is the default SSH port?
3. Why is SSH more secure than Telnet?
4. What is Public Key Authentication?
5. What is the difference between SCP and SFTP?
6. Which command generates an SSH key?
7. Where is the SSH server configuration file located?
8. How do you copy your public key to a server?
9. Which command checks the SSH service status?
10. What are SSH security best practices?

---

# Summary

Topics Covered

- SSH
- SSH Authentication
- Password Authentication
- Public Key Authentication
- SCP
- SFTP
- SSH Configuration
- SSH Commands
- Security Best Practices
- SSH vs Telnet

Common Port

- SSH: 22

Common Commands

- ssh
- ssh-keygen
- ssh-copy-id
- scp
- sftp
- systemctl
- ss

**End of File**
