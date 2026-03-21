## Cybersecurity Firewalls — Summary

### What is a Firewall?
A firewall is a network security device that monitors and controls incoming (ingress) and outgoing (egress) traffic based on defined rules. It helps block unauthorized access while allowing legitimate communication.

---

### Types of Firewalls

#### 1. Traditional Firewall (Layer 4)
- Operates mainly at the Transport Layer (TCP/UDP)
- Performs:
  - Network Address Translation (NAT)
  - Packet filtering (allow/block traffic)
  - Routing and connection tracking
  - VPN support
- Faster and cost-effective but limited in advanced security

#### 2. Next-Generation Firewall (NGFW)
- Provides deeper inspection across multiple OSI layers
- Features:
  - Application awareness and control
  - User and device tracking
  - Intrusion Prevention System (IPS)
  - Encrypted traffic inspection
  - Sandboxing for unknown threats
- Offers enhanced visibility and stronger security

---

### Firewall Administration
- Managed through web interfaces or centralized tools
- Access should be restricted and secured
- Often integrated with identity systems (e.g., Active Directory)

---

### Network Segmentation
- Divides a network into smaller zones
- Controls traffic between segments
- Reduces the spread of attacks
- Flat networks (no segmentation) are less secure
- Supports zero-trust model (no implicit trust)

---

### IDS and IPS
- IDS (Intrusion Detection System): Detects and alerts on threats
- IPS (Intrusion Prevention System): Detects and blocks threats
- Uses signatures and heuristics
- Requires regular updates

---

### Content and Application Filtering
- Identifies and controls applications in traffic
- Filters websites based on categories (e.g., phishing, gambling)
- Can block or warn users via captive portals

---

### Content Control
- Inspects files and data transfers
- Detects malware and data leaks
- Supports multiple protocols (HTTP, FTP, SMTP, etc.)

---

### Sandboxing
- Runs suspicious files in an isolated environment
- Analyzes behavior before allowing access
- Helps detect unknown (zero-day) threats

---

### Traffic Decryption
- Decrypts encrypted traffic for inspection
- Applies to inbound and outbound traffic
- Must consider privacy and legal implications

---

### Unknown Traffic
- Traffic that cannot be identified is labeled as unknown
- Often blocked in high-security environments
