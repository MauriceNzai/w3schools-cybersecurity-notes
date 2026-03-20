# Cybersecurity: Passwords

## Overview
Passwords are a common authentication method but are often weak and vulnerable to attacks such as guessing, reuse, and cracking. This section explores best practices, risks, and modern alternatives.

---

## Password Strength
- Strong passwords depend on **entropy (unpredictability)** rather than just complexity.
- Complex passwords (e.g., `Tr0ub4dor&3`) can still be weak:
  - Hard to remember and type
  - Based on predictable patterns
- **Passphrases** (e.g., `CorrectHorseBatteryStaple`) are better:
  - Easier to remember and type
  - Higher entropy → harder to crack
- Best practice:
  - Use long, meaningful phrases
  - Add variation (capitalization, symbols, spaces)

---

## Password Managers
- Reusing passwords across services is dangerous.
- If one service is compromised, attackers can access others.
- Password managers:
  - Store unique passwords securely
  - Improve productivity (auto-fill, easy access)
  - Enable strong, unique passwords per service
- Even though not perfect, they are safer than password reuse.

---

## Passwordless Authentication
- Alternatives to passwords are emerging:
  - Biometrics (fingerprint, face)
  - Possession-based (phone, token)
- Benefits:
  - Easier for users
  - Reduces password-related risks
- Challenges:
  - Not perfect; trade-offs between usability and security

---

## Multi-Factor Authentication (MFA)
- Adds an extra layer of security beyond passwords.
- Requires:
  - Something you know (password)
  - Something you have or are (code, device, biometrics)
- Examples:
  - Authenticator apps
  - SMS codes
  - Hardware tokens
- Adaptive MFA (DAC):
  - Triggered only in risky situations (new location, sensitive actions)

---

## Password Guessing (Online Attack)
- Attackers try username/password combinations over a network.
- Targets weak or default credentials.
- Common weak passwords:
  - Seasonal passwords (e.g., `Summer2021!`)
  - Company names + simple patterns
  - Personal names and dates
- Tools like Hydra automate guessing attempts.
- Successful guessing can lead to:
  - Account takeover
  - Internal network access
  - Data theft or ransomware

---

## Credential Stuffing
- Uses leaked credentials from breaches.
- Exploits password reuse across services.
- Highly effective due to common user behavior.

---

## Password Cracking (Offline Attack)
- Occurs after attackers obtain password hashes.
- Uses CPU/GPU power to guess passwords.
- Hashing:
  - One-way function for storing passwords securely
- GPUs are faster due to parallel processing.

---

## Services Without Authentication
- Some systems lack authentication entirely.
- Attackers can explore these freely for sensitive data.
- Important during network scanning and enumeration.

---

## Using Existing Credentials
- Attackers reuse already-compromised credentials.
- Methods:
  - Accessing infected systems
  - Dumping credentials (e.g., with tools like Mimikatz)
- Enables lateral movement across systems:
  - Email
  - VPN
  - Internal applications

---

## Key Takeaways
- Prefer **long passphrases over complex short passwords**
- Never reuse passwords across services
- Use a **password manager**
- Enable **multi-factor authentication**
- Be aware of attacks:
  - Password guessing
  - Credential stuffing
  - Password cracking
