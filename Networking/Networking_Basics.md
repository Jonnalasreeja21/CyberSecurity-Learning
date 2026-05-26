# Networking Basics

## Introduction

Networking is the process of connecting computers and devices to communicate and share resources such as files, internet access, printers, and applications.

### Why Learn Networking?

Networking is essential for:

- Cyber Security
- Cloud Computing
- DevOps
- System Administration
- Software Development
- Ethical Hacking

---

# Types of Networks

## PAN (Personal Area Network)

A small network used for personal devices.

**Examples:**
- Bluetooth
- Smartwatch
- Wireless Earbuds

**Range:** 1–10 meters

---

## LAN (Local Area Network)

A network within a small area such as a home, office, or school.

**Examples:**
- Home Wi-Fi
- Computer Labs
- Office Networks

**Advantages:**
- High speed
- Easy management

---

## MAN (Metropolitan Area Network)

A network that covers a city.

**Examples:**
- City-wide ISP networks

---

## WAN (Wide Area Network)

A network that covers large geographical areas.

**Examples:**
- Internet
- International Company Networks

---

# Network Topologies

## Bus Topology

All devices connect to a single cable.

### Advantages
- Low cost
- Easy installation

### Disadvantages
- Single point of failure

---

## Star Topology

All devices connect to a central switch.

### Advantages
- Easy troubleshooting
- Most widely used

### Disadvantages
- Switch failure affects communication

---

## Ring Topology

Devices form a circular connection.

### Advantages
- Organized data flow

### Disadvantages
- Difficult maintenance

---

## Mesh Topology

Every device connects to every other device.

### Advantages
- High reliability

### Disadvantages
- Expensive

---

# OSI Model

The Open Systems Interconnection (OSI) Model consists of 7 layers.

| Layer | Name | Function |
|---------|---------|---------|
| 7 | Application | User Interaction |
| 6 | Presentation | Encryption & Formatting |
| 5 | Session | Session Management |
| 4 | Transport | Reliable Delivery |
| 3 | Network | Routing |
| 2 | Data Link | MAC Addressing |
| 1 | Physical | Hardware Transmission |

## Mnemonic

**Please Do Not Throw Sausage Pizza Away**

- Physical
- Data Link
- Network
- Transport
- Session
- Presentation
- Application

---

# TCP/IP Model

The TCP/IP model is used on the Internet.

| Layer | Protocols |
|---------|---------|
| Application | HTTP, HTTPS, DNS, FTP |
| Transport | TCP, UDP |
| Internet | IP, ICMP |
| Network Access | Ethernet, Wi-Fi |

---

# IP Address

An IP address uniquely identifies a device on a network.

## Example

```text
192.168.1.100
```

## Types of IP Addresses

### Private IP Address

Used inside local networks.

```text
10.0.0.0 - 10.255.255.255
172.16.0.0 - 172.31.255.255
192.168.0.0 - 192.168.255.255
```

### Public IP Address

Used on the Internet.

Example:

```text
8.8.8.8
```

---

# MAC Address

A Media Access Control (MAC) Address is a unique identifier assigned to network interfaces.

Example:

```text
00:1A:2B:3C:4D:5E
```

---

# TCP vs UDP

| Feature | TCP | UDP |
|----------|----------|----------|
| Reliable | Yes | No |
| Speed | Slower | Faster |
| Error Checking | Yes | Limited |
| Connection | Connection-Oriented | Connectionless |

## TCP Examples

- HTTPS
- SSH
- FTP
- SMTP

## UDP Examples

- DNS
- VoIP
- Online Gaming
- Video Streaming

---

# Common Protocols and Ports

| Protocol | Port Number | Purpose |
|------------|------------|------------|
| HTTP | 80 | Web Browsing |
| HTTPS | 443 | Secure Browsing |
| FTP | 21 | File Transfer |
| SSH | 22 | Secure Remote Access |
| DNS | 53 | Domain Name Resolution |
| SMTP | 25 | Email Sending |
| POP3 | 110 | Email Receiving |
| IMAP | 143 | Email Access |

---

# DNS (Domain Name System)

DNS converts domain names into IP addresses.

Example:

```text
google.com → 142.250.x.x
```

Without DNS, users would need to remember IP addresses.

---

# Network Devices

## Router

Connects different networks and forwards data packets.

### Functions
- Internet connectivity
- Routing traffic
- NAT

---

## Switch

Connects devices within a LAN.

### Functions
- MAC address learning
- Frame forwarding

---

## Hub

Broadcasts data to all connected devices.

### Drawback
- Inefficient communication

---

## Firewall

Filters incoming and outgoing network traffic.

### Purpose
- Prevent unauthorized access
- Protect systems from attacks

---

# Common Linux Networking Commands

## Display IP Address

```bash
ip a
```

## Test Connectivity

```bash
ping google.com
```

## DNS Lookup

```bash
nslookup google.com
```

## Trace Route

```bash
traceroute google.com
```

## View Open Ports

```bash
netstat -tulnp
```

---

# What Happens When You Open Google?

1. Browser requests google.com
2. DNS finds Google's IP address
3. TCP connection is established
4. HTTPS secures communication
5. Server sends webpage data
6. Browser renders the webpage

---

# Networking Interview Questions

### What is an IP Address?

An address used to identify devices on a network.

### Difference Between TCP and UDP?

TCP is reliable and connection-oriented, while UDP is faster and connectionless.

### What is DNS?

DNS converts domain names into IP addresses.

### What is a Router?

A device that connects multiple networks.

### What is a Firewall?

A security device that filters network traffic.

---

# Summary

After completing these notes, you should understand:

- Networking Fundamentals
- Types of Networks
- Network Topologies
- OSI Model
- TCP/IP Model
- IP and MAC Addresses
- TCP vs UDP
- DNS
- Network Devices
- Common Networking Commands
- Basic Interview Questions

These concepts form the foundation for Cyber Security, Cloud Computing, DevOps, and System Administration.
