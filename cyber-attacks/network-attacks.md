# Cyber Security: Network Attacks

## 1. Overview of Network Attacks
- Network attacks target services and applications running on a network.
- Exploitation = abusing a service beyond its intended use.
- Goal: Gain control of systems or execute malicious code (RCE).

---

## 2. Attack Surface & Discovery
- Attackers map networks using:
  - Port scanning
  - Asset discovery tools (e.g., EyeWitness)
- Purpose:
  - Identify running services
  - Find weak or vulnerable systems

---

## 3. Buffer Overflow
- Occurs when input exceeds allocated memory space.
- Causes:
  - Lack of input validation
  - Unsafe memory handling (common in C/C++)
- Impact:
  - Overwrites memory (e.g., return pointer)
  - Allows attacker to control CPU execution
- Result:
  - Full system compromise

---

## 4. Vulnerability Scanners
- Automated tools to detect:
  - Known vulnerabilities
  - Misconfigurations
- Key Points:
  - Use predefined plugins
  - Do NOT detect zero-day vulnerabilities
  - Can run with or without authentication

---

## 5. Code Execution & Payloads
- Payload = malicious code delivered after exploitation

### Common Payloads:
- Reverse shell (victim connects to attacker)
- Bind shell (attacker connects to victim)
- Backdoor accounts
- GUI/remote control access
- C2 (Command & Control) communication

---

## 6. Firewalls & Evasion
- Firewalls block incoming connections
- Attackers bypass using:
  - Reverse shells (outbound connections)
- Weakness:
  - Many systems allow outgoing traffic

---

## 7. Command & Control (C2)
- Used for remote control of compromised systems

### C2 Techniques:
- HTTPS traffic (disguised as normal browsing)
- Social media communication
- Cloud platforms (e.g., shared docs)

---

## 8. Network Monitoring & Detection
- Focus: Detect anomalies rather than known attacks

### Indicators:
- Long or unusual connections
- Beaconing (regular check-ins)
- Sudden data spikes (data exfiltration)

### Key Principle:
- Context matters (e.g., trusted IP behaving maliciously)

---

## 9. Peer-to-Peer (P2P) Abuse
- Normal networks: Client → Server
- Attackers use: Client ↔ Client

### Example:
- SMB (port 445) used for spreading attacks
- Indicates possible compromise

---

## 10. Lateral Movement & Pivoting
- After compromise, attackers:
  - Move across systems
  - Explore internal networks

### Definitions:
- Pivoting:
  - Using one compromised system to reach others
- Lateral Movement:
  - Actively exploiting additional systems

### Goal:
- Expand control across the network
