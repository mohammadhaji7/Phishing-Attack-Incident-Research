# Detection Analysis

## Endpoint Detection Assessment

A controlled phishing simulation was conducted using GoPhish against a Windows 11 test environment.

The GoPhish campaign recorded the following activity:

- Emails sent: 1
- Emails opened: 1
- Links clicked: 1
- Credentials/data submitted: 0
- Reporting event: Not confirmed as a distinct GoPhish-tracked event

The Windows endpoint telemetry was reviewed after the controlled interaction.

The Windows Security log was examined for relevant authentication and process-creation events, including Event IDs 4624 and 4688. No process-creation event could be confidently attributed to the browser-based phishing interaction.

Windows Defender Operational logs were also reviewed. No phishing-specific threat detection event, such as Event IDs 1116, 1117, or 1118, was identified.

## Finding

The simulation successfully demonstrated user interaction with the phishing link, but the available default Windows endpoint telemetry did not produce a clear phishing-specific detection.

This demonstrates a detection visibility gap: user interaction with a suspicious URL may occur without generating an immediately identifiable endpoint security alert.

The laboratory results should not be interpreted as evidence that Windows security controls cannot detect phishing activity. Rather, no clearly attributable phishing-specific detection event was observed in the telemetry available during this controlled test.

Additional endpoint telemetry, centralized logging, URL/domain reputation controls, browser security controls, email security controls, and SIEM correlation could improve detection capability.

## Reporting Measurement Limitation

The controlled landing page included a "Report This Email as Suspicious" interaction.

The interaction was validated at the landing-page level, but a distinct GoPhish campaign event was not confirmed for the reporting action.

Therefore, no numerical reporting rate is included in this analysis.

This prevents a client-side page interaction from being incorrectly presented as a GoPhish-measured reporting metric.