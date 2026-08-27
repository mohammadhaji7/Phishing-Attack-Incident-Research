# Controlled Phishing Simulation Scenario

## 1. Scenario Objective

The objective of the controlled laboratory simulation is to demonstrate how a believable business-context phishing message can influence a test user to interact with a fraudulent document-sharing workflow.

The scenario is informed by the IEH Corporation phishing incident while remaining isolated from real organizational systems and users.

The simulation focuses on:

- Business-contact impersonation
- Document-sharing-style phishing
- Controlled landing-page interaction
- Benign user interaction
- Phishing-awareness and reporting behavior
- Campaign interaction measurement

---

## 2. Scenario Background

The real IEH Corporation incident involved an attacker impersonating a prospective business contact and using a fraudulent Microsoft document-sharing communication to obtain employee credentials.

The laboratory simulation reproduces the relevant social-engineering concept in a safe environment.

It does not attempt to reproduce the real incident against IEH or any other organization.

---

## 3. Simulated Phishing Scenario

A designated test user receives a controlled phishing email presented as a business document-sharing request.

The message uses a document-sharing theme intended to appear consistent with normal business communication.

The email contains a link to a controlled laboratory landing page hosted within the isolated test environment.

The landing page presents a benign simulation experience.

---

## 4. Controlled Landing Page

The laboratory landing page is designed to demonstrate the user interaction associated with a phishing workflow.

The page provides controlled actions including:

- **View Shared Document**
- **Report This Email as Suspicious**

The simulation does not collect real credentials.

The landing page is hosted within the controlled laboratory environment.

---

## 5. Benign Interaction

The **View Shared Document** action is used as a benign payload simulation.

The purpose is to demonstrate what could happen after a user follows a phishing link without deploying malware, executing destructive actions, or accessing real sensitive information.

The payload is intentionally harmless and limited to the controlled laboratory environment.

---

## 6. Reporting Interaction

The **Report This Email as Suspicious** action represents the user's security-reporting behavior.

During validation, the action was observed to navigate to the controlled `#report` page section.

The laboratory evidence therefore demonstrates the reporting interaction at the page level.

A reporting percentage will only be included in the final report if GoPhish campaign results provide a distinct tracked reporting event.

If GoPhish does not record the action as a separate campaign event, the report will describe the behavior qualitatively rather than inventing a reporting rate.

---

## 7. Test Environment

The simulation uses:

- Kali Linux
- Windows test environment
- GoPhish
- Controlled test accounts
- Isolated network configuration
- Controlled landing page
- Benign payload
- Authorized laboratory users

The environment is designed for controlled cybersecurity research and demonstration.

---

## 8. Expected User Behaviors

The simulation evaluates whether a designated test user:

1. Receives the simulated phishing email.
2. Interacts with the document-sharing link.
3. Reaches the controlled landing page.
4. Interacts with the benign document action.
5. Recognizes the suspicious nature of the message.
6. Uses the available reporting action.

Only behaviors supported by actual laboratory evidence are treated as measured results.

---

## 9. Metrics

The simulation may provide evidence concerning:

- Campaign delivery
- Email interaction
- Link interaction
- Landing-page interaction
- Benign payload interaction
- Campaign results

A reporting rate will not be stated unless GoPhish records the reporting action as a distinct tracked campaign event.

No fabricated metric will be included.

---

## 10. Safety Controls

The simulation deliberately avoids:

- Real employee targeting
- Unauthorized external targets
- Real passwords
- Real credential harvesting
- Malware
- Destructive payloads
- Unauthorized system access
- Real sensitive organizational information
- Data exfiltration

All testing is conducted within the controlled laboratory environment.

---

## 11. Relationship to the IEH Incident

The simulation reproduces selected characteristics of the IEH incident at a conceptual level:

| IEH Incident | Controlled Simulation |
|---|---|
| Prospective business-contact impersonation | Business-context phishing lure |
| Fraudulent document-sharing communication | Document-sharing-style email |
| Fraudulent authentication workflow | Controlled landing page |
| Credential exposure | Not performed with real credentials |
| Mailbox access | Not reproduced |
| Sensitive information exposure | Not reproduced |
| Malicious mailbox rules | Not reproduced |
| Security awareness/reporting | Reporting action tested |

The simulation therefore demonstrates the initial phishing and awareness aspects of the incident without reproducing unauthorized access or harmful post-compromise activity.

---

## 12. Scope and Limitations

The laboratory simulation is intentionally narrower than the real IEH incident.

It does not reproduce:

- Real Microsoft 365 account compromise
- Real mailbox access
- Export-controlled information
- Malicious mailbox persistence
- Confirmed data exfiltration
- Unauthorized external systems

The purpose is to safely demonstrate phishing behavior and evaluate the effectiveness of basic user-awareness and reporting mechanisms.

---

## 13. Training Objective

The primary training objective is to demonstrate that believable business communications and familiar document-sharing workflows can be used to encourage users to interact with phishing content.

The simulation reinforces the importance of:

- Verifying unexpected document-sharing requests
- Checking links before authentication
- Avoiding credential entry into suspicious pages
- Reporting suspicious messages
- Treating unexpected business communications cautiously
