# Impact Assessment

## 1. Overview

The IEH Corporation phishing incident resulted in unauthorized access to an employee mailbox following a credential-phishing attack.

The affected mailbox contained business and engineering information, including customer communications, purchase-order information, and export-controlled engineering documentation.

The available reporting establishes unauthorized access and the accessibility of sensitive information. It does not establish confirmed exfiltration of that information.

---

## 2. Confidentiality Impact

The primary security impact was to confidentiality.

Following credential compromise, the attacker gained unauthorized access to the affected employee mailbox.

Information accessible through the mailbox included:

- Customer communications
- Purchase-order information
- Export-controlled engineering documentation

The exposure of this information created a potential confidentiality risk because the attacker could access information that was intended for authorized organizational users.

### Assessment

**Confidentiality: High**

The potential sensitivity of the engineering and business information makes unauthorized mailbox access significant even without confirmed data exfiltration.

---

## 3. Integrity Impact

The incident also created a risk to the integrity of mailbox communications and configuration.

The attacker established malicious mailbox rules after gaining access.

Mailbox rules can alter how messages are processed, redirected, hidden, or otherwise handled.

Therefore, unauthorized modification of mailbox configuration represents an integrity concern.

### Assessment

**Integrity: Medium**

The available reporting establishes malicious mailbox-rule creation, but it does not establish widespread alteration of business records or communications.

---

## 4. Availability Impact

The available reporting does not establish a significant availability outage affecting IEH's broader business operations.

The incident was primarily an identity, mailbox-access, and information-confidentiality event.

Securing the affected account and disabling malicious mailbox rules may have temporarily affected the compromised account's normal operation during response, but a broader organizational service outage is not established.

### Assessment

**Availability: Low**

No major organization-wide availability impact is established by the available evidence.

---

## 5. Information and Data Impact

The compromised mailbox contained information of different sensitivity levels.

### Business Information

Customer communications and purchase-order information could provide an attacker with insight into business relationships, transactions, and organizational activities.

### Engineering Information

The mailbox also contained export-controlled engineering documentation.

Unauthorized access to export-controlled information can create significant regulatory, contractual, compliance, and national-security-related concerns depending on the specific information and applicable export-control requirements.

The assessment does not claim that export-controlled information was exfiltrated.

---

## 6. Regulatory and Compliance Significance

The presence of export-controlled engineering documentation increases the potential significance of the incident.

Organizations handling controlled technical information must consider whether unauthorized access creates reporting, investigation, contractual, or regulatory obligations.

The available incident reporting establishes that such information was accessible through the compromised mailbox.

It does not establish the specific downstream regulatory outcome or confirmed transfer of the information.

Therefore, this report treats the regulatory and compliance implications as **potential impact**, rather than claiming a confirmed violation or confirmed disclosure.

---

## 7. Operational Impact

The incident required the organization to take response actions including:

- Securing the affected employee account
- Disabling malicious mailbox rules
- Reviewing the affected mailbox and accessible information
- Reviewing authentication controls

These activities require investigation and security-response resources.

The incident therefore created an operational burden even though a major service outage is not established.

### Assessment

**Operational Impact: Medium**

The assessment reflects the response and investigation effort rather than a quantified financial or productivity loss.

---

## 8. Financial Impact

No specific financial loss is established by the available incident information used in this project.

Unlike incidents involving confirmed fraudulent transactions or ransomware payments, this analysis does not assign a monetary value to the impact without supporting evidence.

Potential financial consequences could arise from investigation, incident response, legal or regulatory requirements, or loss of sensitive business information, but these remain potential consequences rather than confirmed losses.

### Assessment

**Confirmed Financial Loss: Not Established**

---

## 9. Reputational Impact

Unauthorized access to business and engineering information can create reputational risks for an organization.

Potential consequences include:

- Reduced confidence among business partners
- Concerns regarding protection of sensitive information
- Increased scrutiny of security practices
- Potential concerns regarding handling of controlled technical information

However, the available reporting does not provide a quantified measurement of reputational damage.

### Assessment

**Reputational Impact: Potential / Not Quantified**

---

## 10. CIA Triad Assessment

| Security Property | Impact | Reason |
|---|---|---|
| Confidentiality | High | Unauthorized mailbox access exposed business and engineering information, including export-controlled documentation. |
| Integrity | Medium | The attacker established malicious mailbox rules, representing unauthorized modification of mailbox configuration. |
| Availability | Low | No significant organization-wide service outage is established. |

---

## 11. Risk Assessment

The overall significance of the incident is driven primarily by the sensitivity of the information accessible through the compromised mailbox.

The attack demonstrates that a phishing-based identity compromise can create substantial information-security risk without requiring malware or destructive activity.

The presence of export-controlled engineering documentation increases the potential consequences of unauthorized access.

However, the absence of confirmed exfiltration must be maintained as an important evidence limitation.

---

## 12. Evidence Limitations

The following distinctions are important:

### Confirmed

- Phishing-based credential compromise
- Unauthorized access to the affected mailbox
- Accessibility of sensitive business and engineering information
- Presence of malicious mailbox rules
- Account securing and rule removal as response actions

### Not Established

- Confirmed exfiltration of sensitive information
- Confirmed financial loss
- Confirmed organization-wide service outage
- Quantified reputational damage
- Specific downstream regulatory outcome

The report will not convert potential consequences into confirmed impacts without supporting evidence.

---

## 13. Overall Impact Assessment

The IEH incident primarily affected **confidentiality and identity security**.

The compromise provided unauthorized access to a business mailbox containing customer communications, purchase-order information, and export-controlled engineering documentation.

The malicious mailbox rules additionally created an integrity and persistence concern.

The most important impact distinction is that **unauthorized access and information accessibility are established, while confirmed exfiltration is not**.

This distinction prevents the assessment from overstating the consequences of the incident while still recognizing the significance of the information that was accessible to the attacker.