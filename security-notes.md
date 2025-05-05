# SecurityX Exam Preparation Notes

## Core Security Concepts
### CIA Triad
- **Confidentiality**: Preventing unauthorized access to sensitive information
- **Integrity**: Ensuring data remains accurate and unaltered
- **Availability**: Making systems and data accessible to authorized users when needed

### CIANAA (Extended Security Model)
- **Confidentiality**: Protect sensitive data from unauthorized access
- **Integrity**: Ensure data accuracy and reliability
- **Availability**: Maintain system access for authorized users
- **Non-repudiation**: Provide undeniable proof of actions taken
- **Authentication**: Verify identity before access
- **Authorization**: Grant appropriate permissions after authentication


  
## Security Controls
  ### By Function
  - **Preventive**: Block threats before they occur
  - **Detective**: Identify and alert when security events happen
  - **Corrective**: Reduce impact after an incident
  - **Deterrent**: Discourage threat actors
  - **Compensating**: Alternative controls when primary controls aren't feasible

  ### By Implementation Type
  - **Technical Controls**: Hardware/software mechanisms (firewalls, encryption, IDS)
  - **Managerial Controls**: Strategic planning, policies, risk assessments
  - **Operational Controls**: Day-to-day procedures (password policies, awareness training)
  - **Physical Controls**: Tangible security measures (biometrics, surveillance, locks)

## Confidentiality Controls
  ### Data Protection Methods
  - **Encryption**: Convert data into coded format
  - **Access Controls**: Limit who can view sensitive information
  - **Data Masking**: Show only partial information (last 4 digits of SSN)
  - **Physical Security**: Secure physical access to systems
  - **Training**: Educate users on security awareness

### Encryption Applications
- **Communications**: Secure data in transit
- **Storage**: Protect data at rest
- **Authentication**: Secure credential verification

## Integrity Controls
  ### Methods for Ensuring Data Accuracy
  - **Hashing**: Create unique digital fingerprints of data
  - **Digital Signatures**: Combine hashing with encryption using private keys
  - **Checksums**: Verify data integrity during transmission
  - **Anti-tampering**: Prevent unauthorized system modifications
  - **Remote Journaling**: Continuous transmission of transaction logs to secure location

## Availability Controls
  ### Ensuring System Access
  - **Redundancy**:
    - Server redundancy (load balancers, failover configurations)
    - Data redundancy (RAID, hybrid on-premise/cloud systems)
    - Network redundancy (alternate routing paths)
    - Power redundancy (generators, UPS)
  - **Business Continuity Planning**: Strategies for maintaining system availability
  - **Backup Systems**: Regular data backups with tested recovery procedures
  - **Disaster Recovery Testing**: Verify effectiveness of continuity plans

## Authentication (AAA)
  ### Authentication Factors
  - **Something You Know**: Passwords, PINs, security questions
  - **Something You Have**: Smart cards, tokens, mobile devices
  - **Something You Are**: Biometrics (fingerprints, facial recognition)
  - **Something You Do**: Behavioral biometrics, patterns
  - **Somewhere You Are**: Geolocation verification

  ### Multi-Factor Authentication (MFA)
  - Combines two or more authentication factors
  - Significantly increases security posture
  - Essential for protecting high-value assets

## Authorization: permissions or privileges after authentication to protect sensitive data, maintain system integrity, more streamlined user-experience.
  ### Types of Access Control
  - **Role-Based Access Control (RBAC)**: Permissions based on job functions
  - **Rule-Based Access Control**: Permissions based on predefined rules
  - **Mandatory Access Control (MAC)**: System-enforced access based on sensitivity labels
  - **Discretionary Access Control (DAC)**: Owner-defined access permissions
  - **Attribute-Based Access Control (ABAC)**: Dynamic permissions based on attributes

## Accounting
  ### Key Components
  - **Audit Trails**: Chronological records of user actions
  - **Logging**: Recording system and security events
  - **Monitoring**: Continuous observation of system activity

  ### Technologies
  - **Syslog Servers**: Centralized log collection
  - **SIEM Systems**: Security Information and Event Management for real-time analysis
  - **Network Analysis Tools**: Monitor traffic patterns (e.g., Wireshark)


## Non-repudiation
  ### Implementation Methods
  - **Digital Signatures**: Cryptographically secure proof of origin
  - **Secure Audit Logs**: Tamper-evident record keeping
  - **Timestamping**: Cryptographic proof of when actions occurred
  - **Access Controls**: Strict identity and permission management
  - **Regular Audits**: Systematic review of security logs

## Threat and Vulnerability Management
  ### Key Components
  - **Vulnerability Assessment**: Identify and classify system weaknesses
  - **Penetration Testing**: Simulate attacks to test defenses
  - **Threat Intelligence**: Gather information about potential threats
  - **Patch Management**: Systematically apply security updates
  - **Security Awareness**: Train users to recognize and report threats

  ### Metasploit Modules
  - **Auxiliary**: Scanning to identify vulnerabilities
  - **Exploitation**: Gain initial system access
  - **Post-exploitation**: Escalate privileges and explore systems
  - **Payload**: Determine code execution on target
  - **Encoders**: Evade antivirus detection
  - **NOPs**: Generate bytes for payload alignment

## Incident Response
  ### Process Phases
  1. **Preparation**: Develop plans, policies, and response capabilities
  2. **Identification**: Detect and analyze potential incidents
  3. **Containment**: Limit incident impact
  4. **Eradication**: Remove threat from environment
  5. **Recovery**: Restore systems to normal operation
  6. **Lessons Learned**: Document findings and improve process
