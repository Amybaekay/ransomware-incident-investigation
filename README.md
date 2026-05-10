# ransomware-incident-investigation
Incidence response case study focused on ransomware investigation, phishing analysis, and security implementation.

## Overview
This project documents a simulated ransomware incident investigation. The case study
focuses on Orion Health Services, a healthcare technology company that experienced a
ransomware attack following a phishing campaign targeting an employee in the finance
department.
The objective of this investigation was to analyze how the attack occurred, identify the
security weaknesses that contributed to the incident, assess the operational and business
impact, and recommend security improvements to strengthen the organisation’s cybersecurity
posture.

# Incident Summary
The incident began when a finance department employee opened a malicious Excel
attachment delivered through a phishing email. After the attachment was executed, attackers
gained unauthorised access to internal systems and used credential harvesting techniques to
escalate privileges within the environment.
The attackers later deployed ransomware across multiple systems, resulting in encrypted
files, employee lockouts, and operational disruption. Files affected during the attack were
identified with the “.orionlock” extension.
The investigation identified several indicators of compromise, including suspicious overseas
login attempts, unusual outbound network traffic, and evidence of credential dumping
activity using Mimikatz.
Sensitive information impacted during the incident included:
- Employee payroll records
- Patient appointment schedules
- Internal system credentials

# Key Findings
The investigation identified several security weaknesses that contributed to the success of the
attack:
- Limited employee phishing awareness
- Weak email filtering and authentication controls
- Lack of multi-factor authentication (MFA)
- Excessive user privileges
- Insufficient network segmentation

# Recommendations
The following recommendations were proposed to strengthen the security of Orion Health Services’:
- Implement multi-factor authentication (MFA)
- Improve email security using SPF, DKIM, and DMARC
- Conduct regular phishing awareness training
- Deploy Endpoint Detection and Response (EDR) solutions
- Improve centralized logging and monitoring
- Apply least privilege access controls
- Isolate backups from production systems
- Segment critical systems and sensitive environments
- Conduct regular vulnerability assessments and security testing
- Conduct regular backup testing

# Skills Demonstrated
- Incident Response Analysis
- Ransomware Investigation
- Phishing Attack Analysis
- Risk Assessment
- Executive Security Reporting
- Vulnerability Identification
- Security Recommendations
- Business Impact Analysis
- Governance and Compliance Awareness

# Technologies and Concepts Involved
## Cybersecurity Concepts
- Ransomware
- Phishing
- Credential Harvesting
- Privilege Escalation
- Lateral Movement
- Indicators of Compromise (IOCs)
- Incident Response
- Access Control
- Business Continuity

## Security Technologies
- SPF
- DKIM
- DMARC
- Multi-Factor Authentication (MFA)
- Endpoint Detection and Response (EDR)
- Security Information and Event Management (SIEM)

# Disclaimer
This project is based on a simulated cybersecurity scenario completed for educational and
portfolio purposes.
