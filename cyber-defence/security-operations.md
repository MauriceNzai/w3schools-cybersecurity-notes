## Cyber Security – Security Operations

### Overview
Security Operations are typically handled by a SOC (Security Operations Center), responsible for detecting and responding to threats before they escalate into serious incidents.

---

### SIEM (Security Information and Event Management)
- Collects and analyzes logs from:
  - Network
  - Hosts
  - Applications
- **Events**: Observations from logs (e.g., logins, transactions, attacks).
- **Incidents**: Events that pose a real or potential threat.
- SIEM correlates multiple events to generate alerts.
- Application logs provide the most context but often require customization.

---

### SOC Roles
- **SOC Chief**: Defines strategy and defense approach.
- **SOC Architect**: Designs systems and data correlation rules.
- **Analyst Lead**: Develops processes and playbooks.
- **Level 1 Analysts**: First responders to alerts.
- **Level 2 Analysts**: Handle complex issues and escalate incidents.
- **Incident Response Team (IRT)**: Resolves and remediates incidents.
- **Penetration Testers**: Simulate attacks and support defense (Purple Teaming).

---

### Escalation Chains
Defined procedures for handling incidents:
1. Create incident ticket
2. Notify via email/SMS
3. Call primary contact
4. Escalate to secondary contact

---

### Incident Classification
Incidents are categorized by:
- **Category** (e.g., malware, DDoS, insider threat)
- **Criticality** (impact and urgency)
- **Sensitivity** (who should be informed)

---

### SOAR (Security Orchestration, Automation, and Response)
- Automates detection and response processes.
- Helps reduce response time to modern threats.
- Uses technologies like:
  - Infrastructure as Code (IaC)
  - Software Defined Networking (SDN)

---

### Monitoring & Detection
Focus on high-quality, hard-to-evade indicators:
- Easy to change: hashes, IPs, domains
- Hard to change:
  - Tools behavior
  - Tactics, Techniques, and Procedures (TTPs)

Effective security monitoring prioritizes indicators that attackers cannot easily modify.
