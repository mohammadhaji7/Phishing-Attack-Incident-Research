# IEH Corporation Phishing Attack Chain Analysis

## 1. Overview

The IEH Corporation incident involved a targeted phishing attack in which an attacker impersonated a prospective business contact and used a fraudulent Microsoft document-sharing link as the initial lure.

The attack relied primarily on social engineering and credential phishing rather than malware execution. The objective was to persuade an employee to interact with what appeared to be a legitimate business document-sharing request and subsequently enter Microsoft 365 credentials into a fraudulent login page.

The incident demonstrates how a single successful phishing interaction can provide an attacker with access to a business mailbox containing sensitive organizational information.

---

## 2. Attack Chain

### Stage 1 — Business Contact Impersonation

The attacker impersonated a prospective business contact to make the communication appear relevant to the employee's normal business activities.

This increased the credibility of the phishing message because the request was presented within a business context rather than as an obviously suspicious unsolicited message.

**Technique:** Social engineering / trusted-contact impersonation

---

### Stage 2 — Fraudulent Document-Sharing Lure

The employee received a link presented as a Microsoft document-sharing request.

The use of a familiar document-sharing workflow was significant because employees commonly receive legitimate requests to review or access business documents electronically.

The attack therefore relied on contextual trust and familiarity rather than requiring sophisticated malware.

**Technique:** Spear phishing link / document-sharing lure

---

### Stage 3 — Fraudulent Microsoft 365 Login Page

Following the phishing link, the employee was presented with a fraudulent Microsoft 365-style authentication page.

The page was designed to resemble a legitimate authentication workflow and was used to obtain the employee's credentials.

This represents the credential-phishing stage of the attack.

**Technique:** Credential phishing / fraudulent authentication page

---

### Stage 4 — Credential Exposure

The employee entered credentials into the fraudulent authentication page.

This provided the attacker with authentication information that could be used to access the employee's mailbox.

No malware installation was required for this stage of the attack.

---

### Stage 5 — Mailbox Access

Using the compromised credentials, the attacker gained access to the employee's mailbox.

The mailbox contained business information including customer communications and purchase-order information.

The incident therefore moved from an initial phishing interaction into an unauthorized access and information-exposure event.

---

### Stage 6 — Sensitive Information Exposure

Information accessible through the mailbox included:

- Customer communications
- Purchase orders
- Export-controlled engineering documentation

The presence of export-controlled engineering information significantly increased the potential impact of the compromise.

Unauthorized access to such information can create confidentiality, regulatory, contractual, and national-security-related concerns depending on the specific information involved and applicable export-control requirements.

Importantly, the available incident reporting does **not establish confirmed exfiltration of the information**. The analysis therefore treats this as unauthorized access and potential exposure rather than confirmed data theft.

---

### Stage 7 — Malicious Mailbox Rules

The attacker established malicious mailbox rules after gaining access.

Mailbox rules can provide persistence by automatically processing, redirecting, hiding, or otherwise manipulating messages according to attacker-controlled conditions.

In this incident, the malicious rules demonstrated that the compromise was not limited to the initial credential access.

The attacker attempted to maintain useful access to the compromised mailbox through changes to the mailbox environment.

**Technique:** Email collection/persistence through malicious mailbox rules

---

### Stage 8 — Organizational Response

Following discovery of the incident, IEH secured the affected account and disabled the malicious mailbox rules.

The organization also reviewed authentication controls as part of its response.

These actions addressed both the compromised identity and the persistence mechanism identified during the incident.

---

---

## 4. Attack Characteristics

The incident demonstrates several important characteristics of modern phishing attacks.

### Social Engineering

The attacker relied on a believable business scenario rather than an obviously malicious message.

### Credential Phishing

The fraudulent authentication page was used to obtain employee credentials.

### Identity-Based Attack

The compromise of a legitimate employee account provided access to information that would not normally be available to an external attacker.

### Business Email Compromise Risk

Once mailbox access was obtained, the attacker could potentially observe or manipulate business communications and information.

### Persistence

The malicious mailbox rules demonstrated an attempt to maintain useful access to the compromised mailbox after the initial credential compromise.

### Data Confidentiality Risk

The mailbox contained sensitive business and engineering information, including export-controlled documentation.

---

## 5. Key Security Lessons

The IEH incident demonstrates that phishing defenses cannot rely solely on detecting obviously malicious emails.

The attack used:

1. A believable business relationship
2. A familiar document-sharing workflow
3. A trusted-looking authentication experience
4. A legitimate employee identity
5. Access to a valuable business mailbox

This means organizations should combine technical controls with employee awareness, strong authentication, email security, mailbox monitoring, and effective incident-reporting procedures.

---

## 6. Relationship to the Controlled Lab Simulation

The controlled phishing simulation developed for this project reproduces the relevant social-engineering concept in an isolated environment.

The simulation uses:

- GoPhish as the phishing-simulation framework
- A controlled phishing email
- A document-sharing-style lure
- A controlled landing page
- A benign "View Shared Document" action
- A controlled reporting action
- A segmented test-user group
- Campaign interaction metrics

The simulation does not reproduce the IEH incident against real systems or users.

It deliberately avoids:

- Malware
- Executable payloads
- Destructive actions
- Real credential collection
- Unauthorized targets
- Real sensitive information

The purpose is to demonstrate the relevant phishing attack behavior safely and evaluate phishing-awareness controls.

---

## 7. Scope and Limitations

The analysis is based on publicly reported information regarding the IEH incident and evidence collected from the controlled laboratory simulation.

The available reporting establishes unauthorized mailbox access and the presence of sensitive information within the mailbox. It does not establish confirmed exfiltration of that information.

The laboratory does not attempt to reproduce every technical aspect of the real incident. It focuses specifically on the phishing, credential-exposure, landing-page interaction, benign payload, and reporting-awareness components required by the project.

Host-level Sysmon correlation was attempted during the laboratory work, but the available results were inconclusive and therefore are not treated as a confirmed detection result.

---

## 8. Security Significance

The incident demonstrates how phishing can act as an entry point to sensitive organizational information without requiring malware or exploitation of a technical vulnerability.

For organizations handling defense-related engineering information, customer data, and export-controlled material, protection of employee identities and mailboxes is therefore a critical component of information security.

The most important lesson is that the security boundary is not limited to servers and network infrastructure. A compromised employee identity and mailbox can provide an attacker with access to highly valuable information.

---

## 3. Simplified Attack Flow

```text
Prospective Business Contact Impersonation
                    ↓
       Fake Microsoft Document Link
                    ↓
       Fraudulent M365 Login Page
                    ↓
          Employee Credential Entry
                    ↓
             Mailbox Access
                    ↓
       Sensitive Information Exposure
                    ↓
        Malicious Mailbox Rules
             (Persistence)
                    ↓
       Account Secured / Rules Removed
                    ↓
       Authentication Controls Reviewed