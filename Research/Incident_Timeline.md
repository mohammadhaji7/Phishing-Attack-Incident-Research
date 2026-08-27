# IEH Corporation Incident Timeline

## 1. Incident Overview

**Organization:** IEH Corporation

**Incident Discovery:** 4 August 2026

**Public Disclosure:** 6–7 August 2026

**Incident Type:** Targeted Phishing / Credential Phishing / Business Email Compromise Risk

The incident involved a phishing communication in which an attacker impersonated a prospective business contact and used a fraudulent Microsoft document-sharing workflow to obtain employee credentials.

The available reporting establishes the sequence of phishing, credential compromise, unauthorized mailbox access, sensitive information accessibility, malicious mailbox-rule activity, and subsequent containment.

---

## 2. Documented Incident Sequence

### 1. Prospective Business Contact Impersonation

**Event:**

The attacker impersonated a prospective business contact and used a believable business context for the communication.

**Significance:**

The business context increased the credibility of the phishing attempt and provided a plausible reason for the employee to interact with the message.

---

### 2. Fraudulent Document-Sharing Communication

**Event:**

The attacker sent a fraudulent Microsoft document-sharing communication.

The communication directed the employee toward a Microsoft-style authentication experience.

**Significance:**

The phishing attempt relied on a familiar business workflow rather than malware or a destructive payload.

---

### 3. Credential Phishing

**Event:**

The fraudulent authentication page was used to obtain the employee's Microsoft 365 credentials.

**Significance:**

The attacker obtained authentication information that enabled subsequent unauthorized access to the affected mailbox.

---

### 4. Unauthorized Mailbox Access

**Event:**

The attacker gained unauthorized access to the affected employee mailbox.

**Information Accessible:**

- Customer communications
- Purchase-order information
- Export-controlled engineering documentation

**Significance:**

The compromise progressed from credential phishing to unauthorized access to business information.

---

### 5. Sensitive Information Accessibility

**Event:**

Sensitive business and engineering information was accessible through the compromised mailbox.

The mailbox included export-controlled engineering documentation.

**Evidence Limitation:**

Available reporting does not establish confirmed exfiltration of the sensitive information.

The project therefore distinguishes between unauthorized access or accessibility and confirmed data theft.

---

### 6. Malicious Mailbox Rules

**Event:**

The attacker established malicious mailbox rules after gaining mailbox access.

**Significance:**

The rules represented an additional mailbox-level persistence or monitoring mechanism.

The available reporting does not establish the exact time at which the rules were created.

---

### 7. Incident Discovery

**Date:** 4 August 2026

**Event:**

IEH identified unauthorized activity involving the affected employee account.

**Significance:**

The discovery initiated the organization's containment and investigation activities.

---

### 8. Account Containment

**Event:**

IEH secured the affected account.

**Significance:**

Securing the account addressed the compromised identity and reduced the opportunity for continued unauthorized access.

---

### 9. Malicious Rule Removal

**Event:**

IEH disabled the malicious mailbox rules established by the attacker.

**Significance:**

Removing the unauthorized mailbox configuration addressed the identified persistence mechanism.

---

### 10. Authentication Control Review

**Event:**

IEH reviewed authentication controls following the incident.

**Significance:**

The review addressed the authentication component of the compromise and the organization's ability to reduce the risk of similar credential-phishing attacks.

---

### 11. Public Disclosure

**Date:** 6–7 August 2026

**Event:**

The incident was publicly disclosed through IEH's regulatory reporting.

**Significance:**

The disclosure provided formal information concerning the incident, affected account, accessible information, and response actions.

---

## 3. Simplified Incident Timeline

```text
Prospective Business Contact Impersonation
                |
                v
Fraudulent Microsoft Document-Sharing Communication
                |
                v
Fraudulent Microsoft 365 Authentication Page
                |
                v
Employee Credential Exposure
                |
                v
Unauthorized Mailbox Access
                |
                v
Sensitive Business / Engineering Information Accessible
                |
                v
Malicious Mailbox Rules Established
                |
                v
Incident Discovered
        4 August 2026
                |
                v
Affected Account Secured
                |
                v
Malicious Mailbox Rules Disabled
                |
                v
Authentication Controls Reviewed
                |
                v
Public Disclosure
        6–7 August 2026