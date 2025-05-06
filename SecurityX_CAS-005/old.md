The main software Problem: Security vs Usability

    - Information Security: protecting from unauthorized access, modification, disclosure or corruption (data)

    - Information System Security: protecting the systems that hold and process data (devices)


CIA Triad: Confidentiality, Integrity, Availability

Non-repudiation: specific actions have taken place and cannot be denied (lied about happening)

Authentication: Authentication, Authorization, Accounting (AAA)

## Threats and Vulnerabilities

Risks require "Threat + Vulnerability"
    - Types of Vulnerabilities:
        ○ Operational Readiness: Lack of Preparation
        ○ Scheduling Vulnerability
        ○ Vehicular Vulnerability

CIANAA
# Confidentiality: Regulatory compliance 
    - Personally Identifiable Information
    - Personal Health Information
    - Financial Data
    - How to protect?
        ○ Encryption
        ○ Access Controls
        ○ Data Masking (last 4 of SSN) or (last 4 only of CC number)
        ○ Physical Security Measures
        ○ Training and Awareness
        
    - By encrypting communications and documents, the law firm is ensuring the confidentiality of their client information, preventing unauthorized access to sensitive data. 
        ○ Confidentiality: identify and mitigate threats that could lead to unauthorized access and disclosure of sensitive information
                ○ Incident response testing
                    § simulating security breaches to asses and improve an organizations ability
                    In metasploit, there are multiple modules available - e.g., auxillary, exploitation and post exploitation. 
                        □ Auxiliary does scanning to check whether a specific vulnerability is present on a target system, exploitation is used for initial access or foothold and post exploitation is used to escalate privileges and further explore the target system.
                        □ Exploitation modules contain actual exploits for vulnerabilities in specific systems or applications, allowing attackers to gain initial access.
                        □ Post modules are used after successful exploitation to gather additional information, maintain access, pivot to other systems, or escalate privileges.
                        □ There are also payload modules which determine what code runs on the target after successful exploitation.
                        □ Encoders help evade antivirus detection by encoding payloads in different formats.
                        □ NOPs (No Operation) modules generate random bytes to achieve proper payload alignment in memory during exploitation.
                ○ Encryption: Used to protect sensitive data
                ○ Data breach: Unauthorized individuals to confidential information
                ○ Data leak response: Contain an mitigate data breach, document, inform regulatory body
                ○ Reporting:
    - Threat identification and modeling
    - Vulnerability assessment
    - Risk calculation (likelihood × impact)
    - Risk prioritization
    - Risk treatment options (accept, mitigate, transfer, avoid)
    - Implementation of controls
    - Continuous monitoring and reassessment

# Availibility
[*See risk-management.md*](./risk-managment.md#confidentiality)



# Non-repudiation: undeniable evidence action was authentic 
    - Digital Signatures
    - Hashing (converting data into fixed-sized value) -> Hash Digest = Digital Fingerprint
    - Digital Signature (after hashing, use encryption with users PK)
    - Checksums verify integrity of data during transmission
    - Access Controls (AWS IAM, RWX privileges)
    - Regular Audits (Systematically Review Logs)


# Authentication involves confirming identities, not directly protecting data privacy.
*2FA / MFA is a combination of Authentication factors
    - Knowledge Factor (something you know)
    - Possession Factor (something you have)
    - Inherence Factor (something you are) e.g biometric identification
    - Action Factor (something you do) 
    - Location Factor (somewhere you are) NordVpn vs FDU sign in when not in US




# Authorization: permissions or privileges after authentication
    - Role-based
    - Rule-based
    - Protect sensitive data,  maintain system integrity, more streamlined user-experience



# Accounting
    1. Audit Trail: Establishes a chronological record of user actions, aiding in tracing changes and unauthorized access back to specific users.
    2. Regulatory Compliance: Helps organizations adhere to data protection regulations by maintaining comprehensive records.
    3. Forensic Analysis: Detailed logs assist in understanding security breaches and preventing future incidents.
    4. Resource Optimization: Tracking resource usage enables informed decisions about allocation, improving performance and reducing costs.
    5. User Accountability: A robust accounting system fosters user awareness of monitoring, deterring misuse and encouraging compliance with security policies.
The lecture also discusses relevant technologies, including Syslog servers, network analysis tools like Wireshark, and SIEM systems for real-time monitoring. Overall, meticulous record-keeping is essential for transparency, compliance, forensic preparedness, resource management, and ensuring user accountability in cybersecurity.

Security Controls
    1. Technical Controls: These involve hardware and software mechanisms that manage and reduce risk, such as antivirus software, firewalls, and encryption.
    2. Managerial Controls: Also known as administrative controls, these focus on strategic planning and governance, ensuring security aligns with business goals through risk assessments, policies, and training.
    3. Operational Controls: These consist of daily procedures and measures to protect data, like password policies and user awareness training.
    4. Physical Controls: These tangible measures protect assets, including surveillance cameras and secure access protocols.




SIEM: Splunk Enterprise Security, IBM QRadar, Microsoft Sentinel, and SolarWinds Security Event Manager. 
