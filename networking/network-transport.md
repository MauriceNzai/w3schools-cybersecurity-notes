# Cybersecurity: Network Transport Layer

## Overview
The Transport and Link layers are essential for communication between systems on a network. Multiple protocols operate together, each with potential security risks.

---

## TCP (Transmission Control Protocol)
- Uses **ports (0–65535)** to identify services.
- Provides **reliable, ordered, and controlled communication**.
- Key fields:
  - Source & Destination Ports
  - Sequence & Acknowledgment Numbers
  - Control Bits

### TCP 3-Way Handshake
Establishes a reliable connection:
1. **SYN** – Client initiates with a sequence number.
2. **SYN-ACK** – Server acknowledges and responds.
3. **ACK** – Client confirms, completing the connection.

- Uses **pseudo-random sequence numbers (PRNG)** for security.
- Ensures both parties agree to communicate.

---

## Spoofing Traffic
- Attackers can **forge packets** with manipulated headers.
- TCP offers some protection via sequence numbers.
- If sequence numbers are predictable → **connection hijacking possible**.
- Protocols like **UDP and ICMP are more vulnerable**.
- Typically requires **high system privileges (root/admin)**.

---

## UDP (User Datagram Protocol)
- **Connectionless and faster** than TCP.
- Uses ports but:
  - No handshake
  - No sequencing or control bits
- Lower overhead → used in:
  - VoIP
  - Streaming
  - Modern protocols like QUIC
- **Easily spoofed due to lack of built-in security**

---

## Switched Networks
- Devices connect via **switches using MAC addresses** (not IP).
- MAC Address:
  - 6 octets (e.g., FC:F8:AE:12:34:56)
  - First half = Manufacturer (OUI)
- MAC addresses can be **changed (spoofed)** with admin access.

---

## ARP (Address Resolution Protocol)
- Maps **IP addresses → MAC addresses**.
- Uses:
  - ARP cache for quick lookups
- Command:
  - `arp -a` → view ARP table
- Vulnerable to **ARP spoofing attacks**

---

## VLAN (Virtual LAN)
- Segments networks using **VLAN IDs (tags)**.
- Restricts communication to devices within the same VLAN.
- Improves:
  - Security
  - Network organization
