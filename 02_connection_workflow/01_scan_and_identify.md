## 1) Scan and Identify the Wi-Fi Network

### Goal
- Identify the target **SSID**
- Determine which **security protocol** is in use (RSN / WPA2)

### Key Observations to Document
- SSID name  
- Presence of **RSN information** (indicates WPA2)  
- Signal strength (useful for troubleshooting and reliability assessment)

### Report Wording Example
> “The scan revealed SSID *X* using RSN, indicating WPA2 security.”

---

## Aircrack-ng (Conceptual Use)

The primary goal of **Aircrack-ng** is to assess whether a Wi-Fi network’s
security configuration can withstand common attack techniques.

It is typically used in **authorized testing environments**, such as:
- labs
- training ranges
- internal security assessments

### Aircrack-ng Helps Answer Questions Like:
- Is the wireless encryption configured correctly?
- Are weak passwords or legacy protocols in use?
- Can authentication handshakes be abused or replayed?
- Is the network resistant to offline password-guessing attacks?

---

## How Aircrack-ng Works (High Level)

At a conceptual level, Aircrack-ng operates by:

### Observing Wireless Traffic
It passively monitors Wi-Fi communications between clients and access points.

### Capturing Authentication Material
When devices connect to a protected network, cryptographic handshakes occur.
These handshakes can be recorded **without decrypting traffic**.

### Analyzing Encryption Strength
Captured data is analyzed offline to evaluate whether the network password or
encryption method is strong enough to resist guessing or cracking attempts.

### Validating Security Assumptions
The results indicate whether the network relies on:
- strong, unique credentials  
- modern encryption standards  
- proper key management practices  

> Importantly, Aircrack-ng does not magically “break Wi-Fi” —  
> it exposes weaknesses that already exist due to poor configuration or weak passwords.

---
