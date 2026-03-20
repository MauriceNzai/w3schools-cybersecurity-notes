# Network Layer (Cybersecurity)

## Overview
The Network Layer (Layer 3 of the OSI model) is responsible for routing packets between networks. It ensures data travels from source to destination using logical addressing and routing mechanisms.

---

## Internet Protocol (IP)

- IP enables communication across networks (not just within a single network).
- Two main versions:
  - **IPv4** (32-bit addressing)
  - **IPv6** (128-bit addressing)

### Subnetting & Netmasks
- Networks are divided into **subnets** using a **netmask**.
- Netmask determines:
  - Network size
  - Whether traffic stays local or is routed externally
- Example formats:
  - `192.168.0.1/24` → 255.255.255.0

### Private IP Ranges (RFC1918)
- Used internally (not routable on the internet):
  - `10.0.0.0/8`
  - `172.16.0.0/12`
  - `192.168.0.0/16`

### Key Concepts
- **Broadcast Address**: Last IP in a subnet, sends data to all hosts
- **Localhost**: `127.0.0.1` (loopback)
- **Router**: Forwards packets between networks (unlike switches)

---

## Network Communication

- Packets contain headers with:
  - Source IP
  - Destination IP
- If destination is outside LAN:
  - Traffic is sent to the **default gateway (router)**

---

## NAT (Network Address Translation)

- Maps **public IP ↔ private IP**
- Common uses:
  - Allow multiple internal devices to share one public IP
  - Route incoming traffic to correct internal host via ports
- Typically implemented on routers/firewalls

---

## IPv6

- Designed to replace IPv4 due to address exhaustion
- Uses **128-bit addressing** → vastly larger address space
- Format: 8 groups of hexadecimal numbers
- Can be shortened:
  - Remove leading zeros
  - Use `::` for consecutive zeros
- Example:
  - `2a00:1450:400f:80a::200e`

---

## ICMP (Internet Control Message Protocol)

- Used for diagnostics and error reporting
- Common tools:
  - **Ping** → checks host availability
  - **Traceroute** → maps network path
- Attack use-case:
  - **Ping sweep** to discover active hosts :contentReference[oaicite:0]{index=0}

---

## Traceroute

- Identifies routers between source and destination
- Uses:
  - TTL (Time To Live) / Hop Limit
- Process:
  1. Send packet with TTL = 1
  2. Each router decrements TTL
  3. When TTL = 0 → packet dropped, ICMP response sent back
  4. Repeat with increasing TTL to map full path

---

## DNS (Domain Name System)

- Translates domain names → IP addresses
- Process:
  1. Client queries DNS server
  2. Server checks cache
  3. If not found → recursive lookup to authoritative server
- Uses **TTL** to cache results temporarily

---

## DHCP (Dynamic Host Configuration Protocol)

- Automatically assigns network configuration:
  - IP address
  - Subnet
  - Default gateway
  - DNS servers
- Simplifies network management

---

## VPN (Virtual Private Network)

- Provides **encrypted communication** over networks
- Use cases:
  - Secure remote access
  - Hide/masquerade IP address
- Warning:
  - Some free VPNs may log or misuse user data :contentReference[oaicite:1]{index=1}

---

## Key Takeaways

- The Network Layer is crucial for **routing and addressing**.
- Core technologies include:
  - IP, NAT, ICMP, DNS, DHCP, VPN
- Understanding these is essential for:
  - Network troubleshooting
  - Cybersecurity defense
  - Identifying attack techniques
