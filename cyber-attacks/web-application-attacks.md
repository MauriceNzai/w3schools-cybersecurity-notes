# 📡 Wi-Fi Attacks — Summary

## 📘 Overview
- Wi-Fi uses radio signals (IEEE 802.11) for wireless communication.
- Signals are broadcasted → accessible to anyone within range.
- This increases the risk of interception and unauthorized access.

---

## 📡 Wi-Fi Basics
- Networks use **Access Points (APs)** to connect devices.
- Network name = **SSID (Service Set Identifier)**.
- Wireless traffic can be intercepted using antennas.
- Devices and routers may have vulnerabilities (e.g., outdated firmware).

---

## 🔐 Wi-Fi Security Methods
Common protection mechanisms:
- **Open Network** (no security)
- **MAC Address Filtering**
- **Pre-Shared Key (PSK / password)**
- **Enterprise Authentication (centralized / certificates)**

Key attacker techniques:
- **Monitor Mode** → capture packets
- **Packet Injection** → send forged packets

---

## 🚨 Types of Wi-Fi Attacks

### 1. Open Wi-Fi Attacks
- No encryption → traffic visible to attackers.
- Enables:
  - Data sniffing
  - User activity monitoring
- Security depends on user practices (e.g., HTTPS).

---

### 2. Hidden SSID Weakness
- SSID is not broadcast.
- Not secure because:
  - SSID is revealed when devices connect
  - Devices broadcast known networks
- Can be used to track users.

---

### 3. MAC Address Filtering Bypass
- Only approved MAC addresses can connect.
- Weak because:
  - Attackers can sniff valid MAC addresses
  - Then spoof them
- Easily bypassed.

---

### 4. PSK (Password-Based) Attacks
- Uses WPA/WPA2/WPA3 authentication.
- **WEP** is outdated and insecure.
- Attack method:
  - Capture authentication handshake
  - Perform brute-force or dictionary attacks
- Strong passwords improve security.

---

### 5. Enterprise Authentication Attacks
- Uses centralized authentication (e.g., certificates).
- More secure than PSK.
- Downsides:
  - More complex
  - Can introduce new attack surfaces

---

### 6. Fake Access Point (Evil Twin Attack)
- Attacker creates rogue AP with trusted SSID.
- Devices may connect automatically.
- Enables:
  - Traffic interception
  - Man-in-the-Middle (MITM) attacks

---

## ⚠️ Key Takeaways
- Wi-Fi is inherently less secure due to its broadcast nature.
- Hidden SSID and MAC filtering provide weak protection.
- Strong encryption (WPA2/WPA3) is essential.
- Common attacker techniques:
  - Sniffing
  - Spoofing
  - Rogue access points
