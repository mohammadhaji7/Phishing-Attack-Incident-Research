\# Twitter 2020 Incident Timeline



\## Incident



\*\*Organization:\*\* Twitter  

\*\*Incident Date:\*\* 15 July 2020  

\*\*Incident Type:\*\* Social Engineering / Vishing / Phishing



\---



\## Timeline



\### 1. Initial Social Engineering



\*\*Date:\*\* 15 July 2020



\*\*Event:\*\*



Attackers targeted Twitter employees using social-engineering techniques while impersonating Twitter's internal IT/help-desk personnel.



\*\*Evidence Source:\*\*



\- NYDFS Investigation

\- Twitter Official Incident Disclosure



\*\*Observation:\*\*



The attack initially targeted employees rather than directly attacking Twitter's public-facing infrastructure.



\---



\### 2. Phishing / Fake VPN Page



\*\*Event:\*\*



Targeted employees were directed to a fraudulent website designed to resemble Twitter's legitimate VPN login page.



\*\*Evidence Source:\*\*



\- NYDFS Investigation



\*\*Observation:\*\*



The fraudulent page was used to obtain employee login credentials.



\---



\### 3. Credential Compromise



\*\*Event:\*\*



Credentials entered by targeted employees were captured by the attackers.



\*\*Evidence Source:\*\*



\- NYDFS Investigation

\- Twitter Official Incident Disclosure



\*\*Observation:\*\*



The compromised employee credentials provided the attackers with an initial foothold.



\---



\### 4. MFA Interaction



\*\*Event:\*\*



The attackers used obtained credentials against Twitter's legitimate systems, resulting in MFA authentication requests.



\*\*Evidence Source:\*\*



\- NYDFS Investigation



\*\*Observation:\*\*



The incident demonstrates that possession of credentials alone was not the only factor involved; social engineering was also used during the authentication process.



\---



\### 5. Internal Access



\*\*Event:\*\*



The attackers obtained access to Twitter's internal systems and investigated the company's internal environment.



\*\*Evidence Source:\*\*



\- NYDFS Investigation

\- Twitter Official Incident Disclosure

\- SEC Filing



\*\*Observation:\*\*



The initial employee compromise enabled further reconnaissance within the organization's internal environment.



\---



\### 6. Access to Account Support Tools



\*\*Event:\*\*



The attackers targeted employees who had access to internal tools used to support Twitter accounts.



\*\*Evidence Source:\*\*



\- NYDFS Investigation

\- Twitter Official Incident Disclosure



\*\*Observation:\*\*



Access to privileged internal tools significantly increased the potential impact of the initial compromise.



\---



\### 7. Account Compromise and Information Access



\*\*Event:\*\*



The attackers used the internal tools to compromise targeted Twitter accounts and access information associated with some accounts.



\*\*Quantitative Evidence:\*\*



\- 130 accounts targeted

\- 45 accounts used to send Tweets

\- 36 accounts had their direct-message inbox accessed

\- 7 accounts had Twitter data downloaded



\*\*Evidence Source:\*\*



\- Twitter Official Incident Disclosure

\- NYDFS Investigation



\---



\### 8. Financial Impact



\*\*Event:\*\*



The attackers used compromised accounts as part of a cryptocurrency-related fraud campaign.



\*\*Quantitative Evidence:\*\*



More than $118,000 worth of Bitcoin was transferred to attacker-controlled addresses.



\*\*Evidence Source:\*\*



\- NYDFS Investigation



\---



\### 9. Organizational Response



\*\*Event:\*\*



Twitter restricted compromised accounts, revoked access where necessary, investigated the incident, and worked with law enforcement and external investigators.



\*\*Evidence Source:\*\*



\- Twitter Official Incident Disclosure

\- NYDFS Investigation



\*\*Observation:\*\*



The response focused on containment, investigation, restoration of account access, and strengthening security controls.



\---



\## Evidence Classification



\### Source-Derived Facts



Facts directly supported by the cited sources.



\### Our Analysis



Interpretations based on the documented attack sequence.



\### General Security Recommendations



Security controls proposed based on the lessons learned from the incident.



\---



\## Sources



1\. New York Department of Financial Services — Twitter Investigation Report

2\. Twitter — An Update on Our Security Incident

3\. U.S. Securities and Exchange Commission — Twitter Form 10-Q

