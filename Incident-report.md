
## Executive Summary

Orion Health Services experienced a ransomware attack that resulted in unauthorised access
to internal systems, encryption of organizational files, and disruption to business operations.
The investigation determined that the attack originated from a phishing email containing a
malicious Excel attachment sent to an employee within the finance department. Following
execution of the attachment, attackers gained access to the internal environment, harvested
credentials, escalated privileges, and moved laterally across multiple systems before
deploying ransomware.

The incident affected sensitive organizational data, including employee payroll records,
patient appointment schedules, and internal credentials. Several security weaknesses
contributed to the success of the attack, including insufficient phishing awareness, weak
email security controls, lack of multi-factor authentication, and inadequate network
segmentation.

This report outlines the nature of the attack, vulnerabilities exploited, operational impact, and
recommended security improvements.


# Organization Background

Orion Health Services is a healthcare technology provider responsible for managing
operational and healthcare-related information. Due to the sensitive nature of the data
processed by the organization, maintaining strong cybersecurity controls is critical to
business continuity and regulatory compliance.


# Incident Overview

## Incident Type
Ransomware Attack

## Initial Access Vector
Phishing email containing a malicious Excel attachment.

## Affected Departments

- Finance
- Human Resources
- IT Operations

## Systems Affected
- File servers
- HR systems
- Finance systems
- Backup infrastructure

## Data Impacted
- Employee payroll records
- Patient appointment schedules
- Internal credentials


# Attack Analysis

The investigation determined that the incident began when an employee within the finance
department interacted with a malicious Excel attachment received through a phishing email.

Once executed, the attachment enabled attackers to gain unauthorized access to internal
systems. The attackers then used credential harvesting techniques, including Mimikatz, to
dump credentials and escalate privileges within the environment.

Following successful privilege escalation, the attackers moved laterally across the network
and deployed ransomware across multiple systems. Encrypted files were identified using the
“.orionlock” extension.

The investigation also identified suspicious overseas login activity and unusual outbound
network traffic, indicating potential remote access and data compromise activity.


# Indicators of Compromise (IOCs)

The following indicators of compromise were identified during the investigation:

- Suspicious overseas login attempts
- Unusual outbound network traffic
- Credential dumping activity using Mimikatz
- Encrypted files with “.orionlock” extension
- Employee account lockouts
- Ransom note discovered on internal systems


# Security Weaknesses Identified

The investigation identified several security weaknesses that contributed to the success and
spread of the ransomware attack.

## Limited Employee Phishing Awareness
Employees lacked sufficient awareness training to identify and report phishing emails and
suspicious attachments.

## Weak Email Security Controls
The organization’s email security controls were insufficient to prevent phishing emails from
reaching employee inboxes.

Potential missing or improperly configured controls included:
- SPF
- DKIM
- DMARC

## Lack of Multi-Factor Authentication (MFA)
The absence of MFA increased the risk of unauthorized access using compromised
credentials.

## Excessive User Privileges
Attackers were able to escalate privileges and access multiple systems within the
environment.

## Insufficient Network Segmentation
Critical systems were insufficiently segmented, allowing attackers to move laterally within
the network.

## Inadequate Backup Isolation
Backup systems were accessible from the production environment, increasing the impact of
the ransomware deployment.

## Limited Monitoring and Detection
Suspicious authentication activity and unusual outbound traffic were not detected early
enough to prevent escalation.


# Operational Impact

The ransomware attack significantly disrupted business operations.

## Business Disruption
- Employees were locked out of internal systems
- Shared resources became inaccessible
- Payroll and HR operations were disrupted

## Healthcare Service Impact
- Patient scheduling systems were affected
- Operational delays impacted healthcare coordination activities

## IT and Security Impact
- Incident response and recovery activities increased operational workload
- System recovery and restoration efforts were required


# Recommendations

The following recommendations are proposed to strengthen Orion Health Services’
cybersecurity posture and reduce the likelihood of future incidents.

## Strengthen Authentication Controls
- Implement multi-factor authentication (MFA)
- Monitor suspicious authentication activity

## Improve Email Security
- Configure SPF, DKIM, and DMARC
- Deploy advanced phishing and spam filtering

## Enhance Employee Security Awareness
- Conduct regular phishing awareness training
- Perform simulated phishing exercises

## Improve Endpoint and Network Security
- Deploy Endpoint Detection and Response (EDR) solutions
- Implement network segmentation
- Restrict lateral movement between systems

## Strengthen Access Controls
- Apply least privilege access principles
- Limit administrative permissions

## Improve Monitoring and Logging
- Centralize security logging and monitoring
- Implement SIEM solutions for threat detection

## Secure Backup
- Isolate backups from production systems
- Conduct regular backup testing


# Conclusion

The investigation determined that the ransomware attack against Orion Health Services
originated from a phishing campaign targeting an employee within the finance department.

The attack exposed several weaknesses in authentication controls, email security, network
segmentation, and employee security awareness. These weaknesses enabled attackers to gain
unauthorized access, escalate privileges, and deploy ransomware across critical systems.

Implementing stronger preventative, detective, and corrective security controls will
significantly improve the organization’s cybersecurity posture and reduce the likelihood
and impact of future attacks.
