# Phishing Attack Incident Research

## IEH Corporation Phishing Incident — Cybersecurity Research and Controlled Laboratory Simulation

## 1. Project Overview

This project analyzes the August 2026 phishing incident involving IEH Corporation and examines how a targeted business-context phishing attack can progress from social engineering and credential phishing to unauthorized mailbox access and exposure of sensitive organizational information.

The project combines:

1. Incident research based on publicly reported information.
2. Attack-chain and impact analysis.
3. Security-control and root-cause analysis.
4. A controlled phishing simulation using GoPhish.
5. Laboratory evidence collection and validation.
6. Security-awareness and mitigation recommendations.

The practical work was conducted in an isolated and authorized laboratory environment.

---

## 2. Real-World Incident

The selected incident involved IEH Corporation, a defense-related connector manufacturer.

The documented attack involved:

- Impersonation of a prospective business contact.
- A fraudulent Microsoft document-sharing communication.
- A fraudulent Microsoft 365-style authentication page.
- Employee credential compromise.
- Unauthorized access to an employee mailbox.
- Access to customer communications and purchase-order information.
- Accessibility of export-controlled engineering documentation.
- Malicious mailbox rules established by the attacker.
- Account containment and removal of the malicious mailbox rules.
- Review of authentication controls following the incident.

The incident was discovered on 4 August 2026 and publicly disclosed through regulatory reporting on 6–7 August 2026.

Available reporting does not establish confirmed exfiltration of the sensitive information. This project therefore distinguishes between unauthorized access/accessibility and confirmed data theft.

---

## 3. Organizational Context

IEH Corporation operates in the defense-related manufacturing sector and produces electrical connectors and related components used in defense systems.

The organization's business context is relevant to the security analysis because its communications and engineering information may have significant commercial, contractual, and export-control implications.

The presence of export-controlled engineering documentation in an affected mailbox increases the potential confidentiality impact of unauthorized access.

This context explains why protection of employee identities, mailboxes, business communications, and sensitive engineering information is an important security requirement.

---

## 4. Research Sources

The project uses the following sources for the real-world incident:

- U.S. Securities and Exchange Commission — IEH Corporation Form 8-K
- The Register — independent cybersecurity reporting
- Security Affairs — independent cybersecurity reporting
- Cybernews — independent cybersecurity reporting

The SEC filing is treated as the primary regulatory evidence source.

Secondary sources are used to corroborate and contextualize the incident.

Incident facts are distinguished from analytical conclusions and project recommendations.

---

## 5. Controlled Laboratory Simulation

The practical component uses an isolated laboratory environment consisting of:

- Kali Linux
- Windows test environment
- GoPhish
- Authorized test accounts
- Controlled network configuration
- Controlled phishing email
- Controlled landing page
- Benign payload interaction

The simulation reproduces selected characteristics of the IEH phishing scenario at a safe conceptual level.

It does not reproduce the real incident against IEH or any other organization.

---

## 6. Simulated Attack Workflow

The controlled simulation follows this general workflow:

```text
Controlled Business-Context Phishing Email
                |
                v
Document-Sharing-Style Link
                |
                v
Controlled Landing Page
                |
        +-------+-------+
        |               |
        v               v
View Shared       Report Email
Document           as Suspicious
        |               |
        v               v
Benign Interaction  #report Section