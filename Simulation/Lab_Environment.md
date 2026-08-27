# Phishing Simulation Lab Environment

## 1. Objective

The laboratory environment was established to safely demonstrate phishing behavior using authorized test accounts and controlled information.

The environment was designed to reproduce selected phishing and security-awareness behaviors from the IEH Corporation incident without targeting real employees, real organizational systems, or real sensitive information.

---

## 2. Lab Components

| Component | Purpose |
|---|---|
| Windows 11 Test Environment | Controlled endpoint used for the phishing interaction |
| Kali Linux VM | Security testing and GoPhish environment |
| GoPhish | Phishing simulation and campaign tracking |
| Test Email Account | Receives the controlled simulation email |
| Test Browser | Interacts with the controlled landing page |
| Controlled Landing Page | Simulates the phishing interaction safely |
| Benign Payload | Demonstrates post-click interaction without malware |
| Isolated/Test Network Configuration | Provides controlled connectivity between the laboratory systems |
| Project Repository | Stores documentation, evidence, analysis, and project artifacts |

---

## 3. Laboratory Isolation and Safety

The simulation was conducted using authorized laboratory systems and designated test accounts.

The following restrictions were maintained:

- No real employee accounts were targeted.
- No unauthorized external organization was targeted.
- No real passwords were collected.
- No real credentials were harvested.
- No malware was deployed.
- No destructive payloads were used.
- No real sensitive organizational information was used.
- Only controlled test interactions were performed.

The purpose of the environment was cybersecurity research, controlled phishing simulation, and security-awareness evaluation.

---

## 4. Implemented Workflow

The implemented laboratory workflow was:

```text
Kali Linux / GoPhish
        |
        v
Controlled Phishing Email
        |
        v
Authorized Windows Test Account
        |
        v
Controlled Landing Page
        |
        +----------------------+
        |                      |
        v                      v
View Shared Document     Report as Suspicious
        |
        v
Benign Interaction
        |
        v
GoPhish Campaign Results
        |
        v
Endpoint Telemetry Review
        |
        v
Detection and Security Analysis