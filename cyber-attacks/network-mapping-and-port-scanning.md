# Network Mapping & Port Scanning

## 📌 Overview
Network mapping and port scanning are essential techniques in cybersecurity used to discover devices, services, and potential vulnerabilities within a network.

---

## 🔍 1. Network Mapping
Network mapping is the process of identifying devices (hosts) on a network.

### 🎯 Purpose
- Discover active systems
- Understand network structure
- Support asset management
- Identify potential attack surfaces

---

## 🛠️ 2. Nmap (Network Mapper)
Nmap is a powerful tool used for:
- Network discovery
- Port scanning
- Service and OS detection

Used by:
- Security professionals (defensive)
- Attackers (reconnaissance)

---

## 🌐 3. Host Discovery Techniques

### a) Ping Sweep (ICMP)
- Sends ICMP echo requests to hosts
- Identifies active devices

**Limitation:**
- Often blocked by firewalls

---

### b) Advanced Probing (Nmap)
- Uses multiple packet types:
  - ICMP
  - TCP SYN
  - TCP ACK
- Helps bypass firewall restrictions

---

### c) ARP Scanning
- Works within local networks (LAN)
- Maps IP addresses to MAC addresses
- Highly reliable for local discovery

---

## 🚪 4. Port Scanning Fundamentals
Port scanning identifies open ports and running services.

### 🔑 Key Idea:
- Open port = potential entry point

### ⚙️ How it works:
- Sends packets to ports
- Analyzes responses

---

## 🔄 5. TCP vs UDP Scanning

### TCP Scanning
- Reliable and commonly used
- Open port → responds with SYN/ACK

### UDP Scanning
- Slower and less reliable
- Requires specific input for responses
- Often no response (harder to detect)

---

## ⚡ 6. Nmap Scan Types & Features

- **Top Ports Scan** → scans common ports
- **Service Version Detection (-sV)** → identifies service versions
- **Script Scanning (-sC)** → runs safe scripts
- **OS Detection (-O)** → identifies operating system
- **Aggressive Scan (-A)** → enables multiple features
- **IPv6 Scanning (-6)** → scans IPv6 targets

---

## ⏱️ 7. Timing Options (Stealth vs Speed)

| Level | Name       | Description              |
|------|------------|--------------------------|
| T0   | Paranoid   | Very slow, stealthy      |
| T3   | Normal     | Default                  |
| T5   | Insane     | Very fast, noisy         |

### ⚖️ Trade-off:
- Faster scans → more detectable
- Slower scans → stealthier

---

## ⏭️ 8. Skipping Host Discovery
- `-Pn` flag:
  - Skips host discovery
  - Assumes all hosts are active
  - Directly performs port scanning

---

## 🖥️ 9. Zenmap (Nmap GUI)
- Graphical interface for Nmap
- Provides:
  - Visual network maps
  - Easier result interpretation

---

## 🧠 Key Takeaways

- Reconnaissance is the first step in cybersecurity
- Network mapping answers: **"What devices exist?"**
- Port scanning answers: **"What services are exposed?"**
- Both are critical for:
  - Security assessments
  - Vulnerability identification
