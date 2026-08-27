# Root Cause Analysis

## 1. Overview

The IEH Corporation phishing incident resulted from a combination of social engineering, credential phishing, unauthorized mailbox access, and mailbox-level persistence.

The attacker did not need to deploy malware or exploit a technical vulnerability to begin the compromise. Instead, the attack relied on impersonating a prospective business contact and presenting a fraudulent Microsoft document-sharing workflow that appeared relevant to normal business activity.

The incident demonstrates how compromise of a single employee identity can provide access to sensitive organizational information.

---

## 2. Social Engineering and Business-Context Trust

### Root Cause

The attacker impersonated a prospective business contact and used a believable business context to make the communication appear legitimate.

### Why It Mattered

Employees are more likely to interact with communications that appear related to an expected or potential business relationship.

The business context therefore reduced the obvious warning signs that might be present in a generic phishing message.

### Security Lesson

Organizations should train employees to independently verify unexpected business communications, particularly document-sharing requests from unfamiliar or newly introduced contacts.

---

## 3. Fraudulent Document-Sharing Workflow

### Root Cause

The attacker used a fraudulent Microsoft document-sharing communication as the phishing lure.

### Why It Mattered

Document-sharing workflows are common in modern business environments. Familiar branding and expected collaboration patterns can therefore increase the credibility of a malicious link.

### Security Lesson

Users should verify the destination and legitimacy of unexpected document-sharing links before interacting with authentication pages.

---

## 4. Credential Phishing

### Root Cause

The phishing communication directed the employee to a fraudulent Microsoft 365-style authentication page designed to obtain credentials.

### Why It Mattered

Credential phishing allowed the attacker to obtain authentication information without requiring malware or exploitation of an endpoint vulnerability.

### Security Lesson

Organizations should use phishing-resistant authentication where practical and combine it with identity monitoring and conditional-access controls.

---

## 5. Identity and Mailbox Access

### Root Cause

The compromised employee credentials enabled the attacker to gain unauthorized access to the affected mailbox.

### Why It Mattered

The mailbox provided access to business communications and information that was valuable to the organization.

This demonstrates that an employee identity can become a significant security boundary within an organization.

### Security Lesson

Identity security should be treated as a critical component of enterprise security. Compromised accounts should be detected, contained, and investigated rapidly.

---

## 6. Sensitive Information Exposure

### Root Cause

The compromised mailbox contained sensitive business and engineering information, including export-controlled engineering documentation.

### Why It Mattered

Unauthorized access to export-controlled information can create significant confidentiality, regulatory, contractual, and compliance concerns depending on the nature of the information and applicable requirements.

The available incident reporting does not establish confirmed exfiltration of the information.

### Security Lesson

Organizations handling sensitive or export-controlled information should apply strong access controls, monitoring, and incident-response procedures to the identities and systems that can access such information.

---

## 7. Malicious Mailbox Rules

### Root Cause

After gaining mailbox access, the attacker established malicious mailbox rules.

### Why It Mattered

Mailbox rules can be used to automatically process, redirect, hide, or otherwise manipulate messages.

Their presence indicates that the attacker modified the compromised mailbox after obtaining access and attempted to establish continued control or visibility.

### Security Lesson

Identity-compromise investigations should include review of mailbox rules and other account-level configuration changes, not only credential resets.

---

## 8. Detection and Monitoring Opportunities

The incident identifies several areas where defensive monitoring can be valuable:

- Suspicious authentication activity
- Unusual mailbox access
- Unexpected mailbox-rule creation
- Abnormal forwarding or message-processing rules
- Changes to account configuration
- Suspicious document-sharing links
- Credential-phishing indicators

These are defensive control opportunities derived from analysis of the incident. They are not claims that IEH lacked each of these controls.

---

## 9. Root Cause Chain

The incident can be represented as:

```text
Business-Contact Impersonation
          ↓
Believable Document-Sharing Lure
          ↓
Fraudulent Authentication Page
          ↓
Credential Exposure
          ↓
Unauthorized Mailbox Access
          ↓
Sensitive Information Accessibility
          ↓
Malicious Mailbox Rules
          ↓
Potential Continued Access / Visibility
          ↓
Account Secured and Rules Disabled