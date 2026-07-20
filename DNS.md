# DNS (Domain Name System)

## About

The Domain Name System (DNS) is a hierarchical naming system that translates human-readable domain names into IP addresses. It allows users to access websites without remembering numerical IP addresses.

---

# What is DNS?

DNS works like the Internet's phonebook.

Instead of typing an IP address like:

```
142.250.190.78
```

You simply type:

```
www.google.com
```

The DNS server finds the corresponding IP address and connects you to the website.

---

# Why Use DNS?

- Easy to Remember Domain Names
- Faster Internet Browsing
- Eliminates Need to Remember IP Addresses
- Supports Large Networks
- Automatic Name Resolution

---

# How DNS Works

1. User enters a domain name.
2. Browser checks its DNS cache.
3. Request is sent to the DNS Resolver.
4. Resolver contacts Root DNS Server.
5. Root Server directs to the TLD Server.
6. TLD Server directs to the Authoritative DNS Server.
7. Authoritative Server returns the IP Address.
8. Browser connects to the destination server.

---

# DNS Resolution Process

```
User

↓

Browser Cache

↓

DNS Resolver

↓

Root DNS Server

↓

TLD Server (.com, .org, .net)

↓

Authoritative DNS Server

↓

IP Address Returned

↓

Website Opens
```

---

# DNS Components

## DNS Resolver

Receives DNS queries from clients and performs the lookup.

---

## Root DNS Server

The highest level in the DNS hierarchy.

Directs queries to the appropriate Top-Level Domain (TLD) server.

---

## TLD (Top-Level Domain) Server

Handles domain extensions such as:

- .com
- .org
- .net
- .edu
- .gov
- .in

---

## Authoritative DNS Server

Stores the actual DNS records for a domain and returns the final IP address.

---

# Common DNS Record Types

## A Record

Maps a domain name to an IPv4 address.

Example

```
example.com → 192.168.1.10
```

---

## AAAA Record

Maps a domain name to an IPv6 address.

---

## CNAME Record

Creates an alias for another domain.

Example

```
www.example.com

↓

example.com
```

---

## MX Record

Specifies the mail server for a domain.

Used by email services.

---

## NS Record

Identifies the authoritative name servers for a domain.

---

## PTR Record

Performs Reverse DNS Lookup.

IP Address → Domain Name

---

## TXT Record

Stores text information.

Commonly used for:

- SPF
- DKIM
- Domain Verification

---

# DNS Cache

DNS responses are temporarily stored to improve performance and reduce lookup time.

Benefits

- Faster Browsing
- Reduced Network Traffic
- Lower DNS Server Load

---

# Public DNS Servers

| Provider | Primary DNS | Secondary DNS |
|----------|-------------|---------------|
| Google DNS | 8.8.8.8 | 8.8.4.4 |
| Cloudflare DNS | 1.1.1.1 | 1.0.0.1 |
| OpenDNS | 208.67.222.222 | 208.67.220.220 |

---

# Common DNS Commands

Check DNS Resolution

```bash
nslookup google.com
```

Display DNS Information

```bash
ipconfig /displaydns
```

Flush DNS Cache (Windows)

```bash
ipconfig /flushdns
```

Renew IP Address

```bash
ipconfig /renew
```

Linux DNS Lookup

```bash
dig google.com
```

or

```bash
host google.com
```

---

# Advantages

- Easy Name Resolution
- Faster Access to Websites
- Distributed Architecture
- Highly Scalable
- Supports Caching

---

# Disadvantages

- DNS Server Failure Can Affect Browsing
- DNS Spoofing Attacks
- Cache Poisoning Risks
- Lookup Delays if Cache Misses

---

# Real-Life Example

Imagine a mobile phone contact list.

Instead of remembering someone's phone number, you save their name.

Similarly,

```
Name → Domain Name

Phone Number → IP Address
```

DNS converts the domain name into the correct IP address.

---

# Interview Questions

1. What is DNS?
2. What is the full form of DNS?
3. Why is DNS used?
4. Explain the DNS resolution process.
5. What is a DNS Resolver?
6. What is the difference between an A Record and an AAAA Record?
7. What is a CNAME Record?
8. What is the purpose of an MX Record?
9. Which command checks DNS resolution?
10. What is DNS Cache?

---

# Summary

Topics Covered

- DNS
- DNS Hierarchy
- DNS Resolver
- Root Server
- TLD Server
- Authoritative DNS Server
- DNS Records
- DNS Cache
- Public DNS Servers
- DNS Commands

Commands

- nslookup
- dig
- host
- ipconfig /displaydns
- ipconfig /flushdns
- ipconfig /renew

**End of File**
