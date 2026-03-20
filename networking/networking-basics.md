## 📄 Cybersecurity Networking Basics (W3Schools) – Summary

### 🌐 Overview
- Networking knowledge is essential in cybersecurity.
- Communication between computers involves multiple layers and processes.
- The **OSI Model** is used to standardize and understand how data moves across networks.

---

## 🧩 OSI Model (Open Systems Interconnection)

A conceptual framework with **7 layers**:

| Layer | Name         | Function |
|------|--------------|----------|
| 7    | Application  | User-facing network services |
| 6    | Presentation | Data formatting, encryption, compression |
| 5    | Session      | Connection management |
| 4    | Transport    | Reliable data transfer |
| 3    | Network      | Routing and addressing |
| 2    | Data Link    | Device-to-device transfer |
| 1    | Physical     | Physical transmission of data |

### Key Points
- **Layers 7–5:** Software (applications & user interaction)
- **Layer 4:** Link between software and hardware
- **Layers 3–1:** Hardware (network devices & transmission)
- **SDN (Software Defined Networking):** Moves network control to software

---

## 🔝 Layer 7 – Application Layer
- Closest to the user.
- Provides network services to applications.
- Examples: Web browsers, email clients
- Protocols: HTTP, FTP, SNMP

---

## 🔐 Layer 6 – Presentation Layer
- Formats and translates data.
- Handles:
  - Encryption (SSL/TLS)
  - Encoding (ASCII, UTF)
  - Compression (GZip)

---

## 🔄 Layer 5 – Session Layer
- Manages communication sessions.
- Responsibilities:
  - Session setup, maintenance, termination
- Protocols: NetBIOS, SIP, SOCKS

---

## 🚚 Layer 4 – Transport Layer
- Ensures data is delivered correctly.
- Protocols:
  - TCP (reliable)
  - UDP (fast, connectionless)
  - QUIC (modern, efficient)

---

## 🌍 Layer 3 – Network Layer
- Handles packet routing between networks.
- Protocols:
  - IP (IPv4/IPv6)
  - ICMP (error handling, diagnostics)
  - IPSec (secure communication)

---

## 🔗 Layer 2 – Data Link Layer
- Transfers data within the same network.
- Technologies:
  - Ethernet
  - Wi-Fi
  - NDP (IPv6)

---

## ⚡ Layer 1 – Physical Layer
- Transmits raw data as signals.
- Mediums:
  - Electrical (cables)
  - Optical (fiber)
  - Wireless (radio)
- Examples: Bluetooth, Ethernet standards

---

## 🧠 Key Takeaways
- The **OSI model** helps understand how networks operate.
- Each layer has specific roles and protocols.
- Cybersecurity measures can be applied at different layers.
- Understanding networking improves threat detection and defense.
