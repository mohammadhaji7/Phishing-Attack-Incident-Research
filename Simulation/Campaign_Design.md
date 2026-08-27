# Phishing Simulation Campaign Design

## 1. Campaign Objective

The objective of the controlled phishing simulation is to evaluate how an authorized test user interacts with a believable business-context phishing email.

The campaign is informed by the social-engineering characteristics identified in the IEH Corporation phishing incident.

The simulation focuses on:

- Business-context phishing
- Document-sharing-style social engineering
- Controlled link interaction
- Benign landing-page interaction
- Security-reporting behavior
- Campaign interaction measurement

---

## 2. Target Group

The campaign uses only authorized laboratory test accounts.

No real employees, external organizations, or unauthorized recipients are targeted.

The test environment is isolated and controlled for cybersecurity research purposes.

---

## 3. Email Scenario

The simulated email uses a business document-sharing theme.

The message is designed to resemble a legitimate request to access or review a shared document.

The campaign includes:

- A controlled sender identity
- A business-context message
- A controlled phishing link
- A document-sharing-style lure
- No malicious attachment
- No malware

The scenario is based on the relevant phishing characteristics of the IEH incident rather than attempting to reproduce the incident itself.

---

## 4. Landing Page

The phishing link directs the authorized test user to a controlled landing page hosted within the laboratory environment.

The landing page provides controlled interaction options including:

- **View Shared Document**
- **Report This Email as Suspicious**

The landing page does not collect real credentials.

The simulation is designed to demonstrate user interaction without compromising real accounts or systems.

---

## 5. Benign Payload

The **View Shared Document** action represents a benign payload interaction.

It is intentionally harmless and does not deploy malware, execute destructive actions, or access sensitive information.

The purpose is to demonstrate the type of interaction that can occur after a user follows a phishing link while maintaining a safe laboratory environment.

---

## 6. Reporting Behavior

The **Report This Email as Suspicious** action represents the user's security-reporting behavior.

During validation, the action was observed to navigate to the controlled `#report` page section.

This demonstrates that the reporting interaction works at the landing-page level.

However, a reporting percentage will only be included in the final analysis if GoPhish campaign results confirm that the reporting action was recorded as a distinct tracked event.

No reporting metric will be estimated or fabricated.

---

## 7. Campaign Metrics

The campaign results are based only on events actually recorded by the laboratory and GoPhish.

Potentially measurable metrics include:

| Metric | Measurement Purpose |
|---|---|
| Email delivery | Confirm campaign delivery |
| Email interaction | Determine whether the test email was accessed, where supported |
| Link click | Measure interaction with the controlled phishing link |
| Landing-page interaction | Confirm access to the simulated phishing page |
| Benign payload interaction | Determine whether the document action was selected |
| Reporting event | Determine whether the reporting action was separately tracked |
| Reporting rate | Calculated only if a distinct GoPhish reporting event exists |

If a metric is not supported by the available evidence, it will be reported as unavailable rather than estimated.

---

## 8. Campaign Results

The campaign results are documented using the available GoPhish campaign evidence and laboratory screenshots.

The project does not claim additional campaign activity that is not supported by the recorded evidence.

The final report will distinguish between:

- Events confirmed by GoPhish
- Events observed directly during browser validation
- Events that could not be independently measured

---

## 9. Reporting Rate Limitation

The reporting interaction requires specific validation because the **Report This Email as Suspicious** button currently navigates to the controlled `#report` page section.

A page-level navigation event does not by itself prove that GoPhish recorded a separate reporting event.

Therefore:

**Reporting Rate = Reported Emails / Emails Delivered × 100**

will only be calculated if the GoPhish campaign results contain a distinct tracked reporting event.

If no such event exists, the final report will describe the reporting behavior qualitatively and state that a reliable reporting rate was unavailable.

---

## 10. Evidence Collection

Evidence collected for the campaign includes:

- GoPhish configuration
- Email template
- SMTP/email delivery evidence
- Controlled landing page
- Benign payload interaction
- GoPhish campaign results
- Reporting behavior validation
- Test-user group configuration

Screenshots are organized within the project `Screenshots` directory according to the documented project structure.

---

## 11. Safety Controls

The campaign remains strictly controlled and authorized.

The simulation does not use:

- Real employee accounts
- Unauthorized recipients
- Real passwords
- Real credential harvesting
- Malware
- Destructive payloads
- Unauthorized system access
- Real sensitive organizational information
- Data exfiltration

All interactions are performed within the controlled laboratory environment.

---

## 12. Relationship to the IEH Incident

The campaign reproduces selected characteristics of the IEH phishing incident at a safe conceptual level.

| IEH Incident | Controlled Campaign |
|---|---|
| Prospective business-contact impersonation | Business-context phishing lure |
| Fraudulent document-sharing communication | Document-sharing-style email |
| Fraudulent Microsoft authentication workflow | Controlled landing page |
| Credential compromise | Not performed using real credentials |
| Mailbox access | Not reproduced |
| Sensitive information exposure | Not reproduced |
| Malicious mailbox rules | Not reproduced |
| Security awareness/reporting | Reporting interaction tested |

The campaign therefore evaluates the initial phishing and user-awareness aspects without reproducing the harmful post-compromise stages of the real incident.

---

## 13. Scope and Limitations

The campaign is intentionally narrower than the real IEH incident.

It does not attempt to reproduce:

- Microsoft 365 account compromise
- Real mailbox access
- Export-controlled information access
- Malicious mailbox persistence
- Confirmed data exfiltration
- Unauthorized external systems

The campaign is a controlled cybersecurity simulation designed to demonstrate phishing behavior and evaluate available awareness and reporting mechanisms.

---

## 14. Final Assessment

The controlled campaign successfully provides laboratory evidence for the phishing workflow, landing-page interaction, benign user interaction, and reporting behavior at the page level.

GoPhish campaign results are used wherever they provide measurable evidence.

Where a behavior cannot be independently recorded as a GoPhish event, the final report will explicitly identify the limitation rather than assigning an unsupported numerical value.

