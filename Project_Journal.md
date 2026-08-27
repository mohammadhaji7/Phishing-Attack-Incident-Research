# Project Journal

## Day 1 — Project Initialization

**Date:** 18 August 2026

### Objective

Initialize the project workspace for the research project on a phishing attack incident that led to sensitive information being exposed.

### Work Performed

* Created the project directory.
* Created folders for research, incident analysis, simulation, metrics, detection, security controls, screenshots, documentation, reports, presentation, references, and policies.
* Created the initial README.md and Project_Journal.md files.
* Initialized the Git repository.
* Created the main branch.
* Configured Git identity.

### Tools Used

* Windows PowerShell
* Git

### Result

The initial project workspace was created successfully.

### Screenshot References

* Screenshots/01_Setup/01_project_structure.png

### Problems Encountered

No significant implementation problem was recorded during project initialization.

### Resolution

Not applicable at project initialization.

### Key Takeaway

The project was structured around a workflow of:

Requirement → Research → Implementation → Testing → Result → Observation → Evidence → Analysis → Recommendation → Documentation

Practical work, measurements, screenshots, challenges, and observations were recorded as the project progressed.

---

## 19 August 2026 — Phishing Simulation Lab Setup

### Work Performed

* Completed the initial incident research and analysis documentation.
* Compared GoPhish, King Phisher, and SET as phishing-simulation tools.
* Selected GoPhish for the controlled laboratory simulation.
* Configured the Kali Linux VM to use VirtualBox NAT networking.
* Verified Kali Linux internet connectivity.
* Downloaded GoPhish v0.12.1 from the official GitHub release.
* Verified the SHA-256 checksum successfully.
* Extracted GoPhish and inspected the default configuration.

### Result

The laboratory environment and phishing-simulation framework were prepared for practical configuration.

### Screenshot References

* Screenshots/01_Setup/01_Kali_Network_Configuration.png
* Screenshots/01_Setup/03_Windows_to_Kali_Connectivity.png
* Screenshots/01_Setup/04_Kali_to_Windows_Connectivity.png
* Screenshots/02_Tool_Configuration/05_GoPhish_Dashboard.png

---

## Practical Implementation — GoPhish Configuration

### Work Performed

* Configured and started the GoPhish phishing-simulation platform.
* Verified that the GoPhish administrative interface was accessible.
* Verified the required GoPhish services were listening.
* Created the controlled phishing email template.
* Configured the controlled landing page.
* Configured the authorized test-user group.
* Configured the campaign within the isolated laboratory environment.
* Tested SMTP/email delivery.
* Captured evidence of the simulated email and campaign configuration.

### Evidence

The following evidence was collected:

* GoPhish dashboard
* GoPhish service/listening state
* Email template configuration
* Detailed email-template configuration
* SMTP/email capture
* Authorized test-user group

---

## Controlled Landing Page Validation

### Work Performed

* Opened the controlled phishing landing page from the Windows test environment.
* Verified that the landing page loaded successfully.
* Verified the **View Shared Document** interaction.
* Verified the **Report This Email as Suspicious** interaction.
* Confirmed that the reporting action navigated to the controlled `#report` page section.
* Confirmed that the training/document interaction navigated to the controlled `#training` page section.

### Observation

The two landing-page actions function as controlled page-level interactions.

The `#report` navigation demonstrates that the reporting interface works at the browser/page level.

However, page-level navigation alone does not prove that GoPhish recorded the reporting action as a separate campaign event.

Therefore, a numerical reporting rate is not included unless the GoPhish campaign results provide a distinct tracked reporting event.

### Evidence

* Screenshots/04_Landing_Page/09_Windows_Phishing_Landing_Page.png
* Screenshots/04_Landing_Page/12_Initial_Landing_Page.png
* Screenshots/08_Reporting_Behavior/15_View_Shared_Document_Training.png
* Screenshots/08_Reporting_Behavior/16_Report_Email_Suspicious.png

---

## Benign Payload Validation

### Work Performed

* Tested the controlled **View Shared Document** interaction.
* Verified the benign payload landing page.
* Verified the resulting benign payload behavior.
* Confirmed that no malware or destructive payload was used.

### Safety Observation

The payload was intentionally limited to a harmless laboratory interaction.

No real credentials, malware, destructive actions, or unauthorized access were used.

### Evidence

* Screenshots/05_Benign_Payload/13_Benign_Payload_Landing_Page.png
* Screenshots/05_Benign_Payload/14_Benign_Payload_Result.png

---

## Campaign Results and Evidence Collection

### Work Performed

* Conducted the controlled campaign using authorized test accounts.
* Reviewed the GoPhish campaign results.
* Captured campaign-result evidence.
* Organized evidence into the project screenshot structure.
* Created a final-evidence folder containing selected evidence from the campaign.

### Evidence

* Screenshots/07_Campaign_Metrics/10_GoPhish_Campaign_Result.png
* Screenshots/09_Final_Evidence/10_GoPhish_Campaign_Result.png
* Screenshots/09_Final_Evidence/14_Benign_Payload_Result.png
* Screenshots/09_Final_Evidence/16_Report_Email_Suspicious.png

### Measurement Limitation

Only metrics directly supported by the GoPhish campaign results are treated as measured results.

The reporting interaction is currently confirmed at the page-navigation level. A reporting percentage will not be fabricated if GoPhish does not record it as a distinct tracked event.

---

## Documentation Correction and Incident Alignment

### Work Performed

The project documentation was reviewed for consistency with the selected IEH Corporation incident.

Several earlier documents contained material based on the previously selected Twitter 2020 incident. Those sections were rewritten rather than simply replacing the organization name.

The following areas were aligned with the IEH incident:

* Incident sources
* Incident timeline
* Attack chain
* Impact assessment
* Response and mitigation
* Root-cause analysis
* Controlled simulation scenario
* Campaign design

### Key Correction

The project analysis now reflects the documented IEH attack characteristics:

Prospective Business Contact Impersonation  
↓  
Fraudulent Microsoft Document-Sharing Communication  
↓  
Fraudulent Microsoft 365 Authentication Page  
↓  
Credential Exposure  
↓  
Unauthorized Mailbox Access  
↓  
Sensitive Information Accessibility  
↓  
Malicious Mailbox Rules  
↓  
Account Containment and Rule Removal

The project does not claim the vishing, internal administrative-tool access, or verified-account takeover mechanics associated with the previously selected Twitter incident.

---

## Documentation and Evidence Organization

### Work Performed

The screenshot evidence was reorganized into the following structure:

```text
Screenshots/
├── 01_Setup/
├── 02_Tool_Configuration/
├── 03_Email_Simulation/
├── 04_Landing_Page/
├── 05_Benign_Payload/
├── 06_Target_Segmentation/
├── 07_Campaign_Metrics/
├── 08_Reporting_Behavior/
└── 09_Final_Evidence/