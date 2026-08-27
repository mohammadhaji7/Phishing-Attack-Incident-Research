# Phishing Simulation Tool Comparison

## 1. Objective

Three phishing simulation and security-testing tools were considered for the controlled laboratory simulation:

- GoPhish
- King Phisher
- Social Engineer Toolkit (SET)

The comparison focuses on suitability for this project rather than general tool capability.

---

## 2. Comparison

| Criteria | GoPhish | King Phisher | SET |
|---|---|---|---|
| Primary purpose | Phishing simulations and awareness testing | Phishing/security awareness campaigns | Social-engineering security testing |
| Campaign management | Strong | Strong | Limited compared with dedicated simulation platforms |
| Email campaign support | Yes | Yes | Yes |
| Landing pages | Yes | Yes | Yes |
| Tracking/metrics | Strong | Strong | More limited for this project's requirements |
| Reporting | Strong | Strong | More limited |
| Ease of use | High | Moderate | Moderate |
| Suitable for controlled awareness testing | Excellent | Good | Good |
| Best fit for this project | High | Medium | Medium |

---

## 3. GoPhish

### Advantages

- Designed specifically for phishing-awareness simulations.
- Provides campaign management.
- Supports email templates and landing pages.
- Provides measurable campaign results.
- Suitable for controlled laboratory testing.
- Results can support quantitative analysis.

### Limitations

- Requires configuration of the email delivery environment.
- Must be operated only in an authorized and controlled environment.
- Does not replace enterprise email-security or SIEM platforms.

---

## 4. King Phisher

### Advantages

- Designed for authorized phishing simulations.
- Supports campaign management and tracking.
- Provides phishing-awareness testing capabilities.

### Limitations

- Deployment and configuration can be more involved.
- It was not selected for the practical implementation because GoPhish better matched the project's requirement for a simple and measurable laboratory experiment.

---

## 5. Social Engineer Toolkit (SET)

### Advantages

- Provides broad social-engineering testing capabilities.
- Useful for security assessments and demonstrations.
- Available in common penetration-testing environments.

### Limitations

- Has a broader security-testing focus rather than being primarily an awareness-campaign management platform.
- It was not selected because GoPhish better matched the structured campaign and measurement requirements of this project.

---

## 6. Tool Selection

### Selected and Implemented Tool: GoPhish

GoPhish was selected and implemented for the practical phase because it closely matched the project's requirements:

- Controlled phishing campaign
- Safe landing pages
- Authorized test accounts
- Campaign tracking
- Quantitative campaign metrics
- Evidence collection

GoPhish was successfully configured and used during the controlled laboratory simulation.

King Phisher and SET remained evaluated alternatives and were not implemented in the practical simulation.

---

## 7. Practical Validation

The selected GoPhish implementation was validated through the controlled laboratory workflow.

The practical implementation included:

- GoPhish configuration
- Email template configuration
- Controlled landing page
- Authorized test-user group
- Campaign execution
- Campaign result collection
- Evidence capture

The campaign successfully recorded the controlled email interaction and link interaction.

Observed campaign results included:

- Emails sent: 1
- Emails opened: 1
- Links clicked: 1
- Credentials/data submitted: 0

The reporting interaction was validated at the landing-page level, but a distinct GoPhish-tracked reporting event was not confirmed. Therefore, no numerical reporting rate is presented.

---

## 8. Safety Considerations

The selected tool was used only within an authorized laboratory environment.

The practical implementation used:

- Authorized test accounts
- Controlled information
- Isolated/test systems
- Controlled recipients
- Benign interactions

Real passwords, real credential harvesting, unauthorized external targets, malware, and destructive payloads were not used.

---

## 9. Conclusion

GoPhish provided the best fit for this project because it combined phishing-campaign management, controlled landing pages, campaign tracking, measurable interaction results, and straightforward evidence collection.

The practical implementation confirmed that GoPhish was suitable for the controlled phishing-awareness experiment.

King Phisher and SET were retained as evaluated alternatives but were not used in the laboratory implementation.
