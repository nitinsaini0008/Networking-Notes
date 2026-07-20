# HTTP & HTTPS

## About

HTTP (HyperText Transfer Protocol) and HTTPS (HyperText Transfer Protocol Secure) are application-layer protocols used for communication between web browsers and web servers.

HTTP transfers data in plain text, while HTTPS encrypts data using SSL/TLS to provide secure communication.

---

# What is HTTP?

HTTP is a protocol used to transfer web pages, images, videos, APIs, and other resources over the Internet.

Example

```
Browser

↓

HTTP Request

↓

Web Server

↓

HTTP Response

↓

Browser Displays Website
```

---

# Default Port

| Protocol | Port |
|----------|------|
| HTTP | 80 |
| HTTPS | 443 |

---

# HTTP Request-Response Cycle

1. User enters a website URL.
2. Browser performs DNS lookup.
3. Browser connects to the web server.
4. Browser sends an HTTP Request.
5. Server processes the request.
6. Server sends an HTTP Response.
7. Browser displays the webpage.

---

# HTTP Request Structure

A request consists of:

- Request Line
- Headers
- Blank Line
- Optional Body

Example

```http
GET /index.html HTTP/1.1
Host: www.example.com
User-Agent: Chrome
Accept: text/html
```

---

# HTTP Response Structure

A response contains:

- Status Line
- Headers
- Blank Line
- Response Body

Example

```http
HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 1200
```

---

# HTTP Methods

## GET

Retrieves data from the server.

Example

```
View a webpage
```

---

## POST

Sends data to the server.

Example

```
Submit Login Form
```

---

## PUT

Updates an existing resource.

---

## DELETE

Deletes a resource.

---

## PATCH

Partially updates a resource.

---

## HEAD

Returns only headers.

---

## OPTIONS

Shows supported HTTP methods.

---

# Common HTTP Status Codes

## 1xx – Informational

Example

```
100 Continue
```

---

## 2xx – Success

| Code | Meaning |
|------|---------|
|200|OK|
|201|Created|
|204|No Content|

---

## 3xx – Redirection

| Code | Meaning |
|------|---------|
|301|Moved Permanently|
|302|Found|
|304|Not Modified|

---

## 4xx – Client Errors

| Code | Meaning |
|------|---------|
|400|Bad Request|
|401|Unauthorized|
|403|Forbidden|
|404|Not Found|

---

## 5xx – Server Errors

| Code | Meaning |
|------|---------|
|500|Internal Server Error|
|502|Bad Gateway|
|503|Service Unavailable|

---

# What is HTTPS?

HTTPS is the secure version of HTTP.

It encrypts all communication between the browser and the server using SSL/TLS.

Example

```
https://www.google.com
```

---

# SSL/TLS

SSL (Secure Sockets Layer) is the older security protocol.

TLS (Transport Layer Security) is the modern and more secure version.

Functions

- Encryption
- Authentication
- Data Integrity

---

# SSL/TLS Handshake

1. Client connects to server.
2. Server sends SSL/TLS Certificate.
3. Client verifies the certificate.
4. Encryption keys are exchanged.
5. Secure communication begins.

---

# Digital Certificate

A Digital Certificate proves the identity of a website.

Contains

- Domain Name
- Public Key
- Certificate Authority
- Expiry Date
- Digital Signature

---

# Certificate Authority (CA)

A Certificate Authority issues and verifies SSL/TLS certificates.

Examples

- DigiCert
- Let's Encrypt
- GlobalSign
- Sectigo

---

# HTTP vs HTTPS

| Feature | HTTP | HTTPS |
|---------|------|-------|
|Port|80|443|
|Encryption|No|Yes|
|Security|Low|High|
|SSL/TLS|No|Yes|
|Data Protection|No|Yes|
|Recommended|No|Yes|

---

# Advantages of HTTPS

- Encrypted Communication
- Secure Login
- Protects Sensitive Data
- Improves User Trust
- Better SEO Ranking

---

# Disadvantages of HTTPS

- Slightly Higher Server Overhead
- Certificate Management Required
- SSL/TLS Certificate Renewal Needed

---

# Common Commands

Check HTTP Headers

```bash
curl -I https://example.com
```

Download a Web Page

```bash
curl https://example.com
```

Test HTTPS Connection

```bash
openssl s_client -connect example.com:443
```

---

# Real-Life Example

Imagine sending a letter.

HTTP

```
Letter without an envelope.
Anyone can read it.
```

HTTPS

```
Letter inside a locked envelope.
Only the intended recipient can read it.
```

---

# Interview Questions

1. What is HTTP?
2. What is HTTPS?
3. What is the difference between HTTP and HTTPS?
4. Which ports are used by HTTP and HTTPS?
5. What is SSL/TLS?
6. What is a Digital Certificate?
7. What is a Certificate Authority (CA)?
8. Explain the HTTP Request-Response Cycle.
9. Name five common HTTP methods.
10. What does a 404 status code mean?

---

# Summary

Topics Covered

- HTTP
- HTTPS
- HTTP Methods
- HTTP Request
- HTTP Response
- Status Codes
- SSL/TLS
- Digital Certificates
- Certificate Authorities
- HTTP vs HTTPS

Common Ports

- HTTP: 80
- HTTPS: 443

Common Commands

- curl
- openssl

**End of File**
