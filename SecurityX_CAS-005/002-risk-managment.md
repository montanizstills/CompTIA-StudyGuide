# Confidentiality, Integrity, Availibility, and Privacy Risk Considerations
## Confidentiality 
<insert>

## Integrity: 
`(relates to the accuracy and reliability of data, not its protection from unauthorized access.)`

    - Integrity Risk Consideration
        • Taken to protect data and systems to unauthorized modifications that could comprise accuracy and trust-worthiness
            ○ Interference
                § Unauthorized alteration or disruption of data or systems leading to integrity  issues 
            ○ Hashing 
                § Cryptographic process that converts data into a fixed-size string of chars. Creates a unique fingerprint to make sure data hasn't been altered.
            ○ Remote journaling
                § Continuous transmission to transaction logs to a remote location
                § Secure backup that helps recover form integrity breaches 
            ○ Anti-tampering
                § Unauthorized changes to hardware or software. Ensure that systems remain trustworthy.
                
    - Availability Risk and Considerations 
        • Ensure that critical systems and data remain accessible and after disruptive events
    
    - Backup Sites:

        A hot site is a fully operational backup facility with hardware, software, and network systems that are continuously running and synchronized with the primary site. Key characteristics include:

        Readiness: Always operational and ready for immediate use
        Data synchronization: Real-time or near real-time data replication
        Recovery time: Minimal (typically minutes to hours)
        Cost: Highest of all options due to duplicate infrastructure and constant maintenance
        Use case: Critical systems where downtime must be minimized, such as financial systems, healthcare, or e-commerce

        Warm Sites
        A warm site is a partially equipped backup facility with core hardware and infrastructure in place, but not fully configured for immediate operation. Key characteristics include:

        Readiness: Partially ready with core infrastructure but requires some setup
        Data synchronization: Periodic backups (typically daily or weekly)
        Recovery time: Moderate (typically hours to days)
        Cost: Medium, balancing readiness and expense
        Use case: Important but non-critical systems where some recovery time is acceptable

        Cold Sites
        A cold site is a backup facility with basic infrastructure (power, connectivity, environmental controls) but minimal or no pre-installed computing equipment. Key characteristics include:

        Readiness: Basic facility only; requires full setup before use
        Data synchronization: Backups must be transported and restored
        Recovery time: Longest (typically days to weeks)
        Cost: Lowest recurring expense
        Use case: Systems where extended recovery time is acceptable or for organizations with limited disaster recovery budgets

    
            ○ Business Continuity Planning
                □ Strategies to maintain availably or to quickly restore systems following disasters
            ○ Backups
                □ Key to recovery in situations once plans and policies are developed
            ○ Business and Continuity Disaster Recovery Testing
                □ Verify processes in place can be effectively executed
        • FAIR (Factor Analysis of Information): Focuses on financial impact as away to prioritize risk.
    
## Privacy Risk Considerations: 
    - includes Biometric, data subject rights and data sovereignty
    - Data subjects are owners of data collected in store
    - Data subject rights to access, correct or delete their own data.
    - Data  sovereignty is laws that govern laws to data.

## Privacy Risk Management
  ### Considerations
  - **Data Subject Rights**: Access, correction, deletion of personal data
  - **Data Sovereignty**: Compliance with jurisdiction-specific data laws
  - **Biometric Data**: Special handling of uniquely identifying physical characteristics
  - **Data Minimization**: Collect only necessary information
  - **Retention Policies**: Define how long data is kept


## Availability Risk Considerations: 
`(is about ensuring data is accessible to authorized users when needed, not protecting it from unauthorized access.)`

    - Redundancy
        ○ Server Redundancy (Load Balancers or Failover Configuration)
        ○ Data Redundancy (Store data in multiple places, i.e. RAIDS or Hybrid on-premise / cloud based systems)
        ○ Network Redundancy (if on network path fails, data can travel via alt route)
        ○ Power Redundancy (generators or other uninterrupted power supplies)

## Third-Party Risk Management: 
`(involves assessing and mitigating risk associated with parities that provide data or services)`

### Risk(s)
- Vendor risk: Vendor security assessment
- Supply Chain risks: Supply chain risk analysis
- Contractual security requirements
- Ongoing monitoring and auditing
- Incident response coordination
- Exit strategies and contingency planning
- Subprocess/subcontractor risks

### Key Processes
- **Vendor Security Assessment**: Evaluate security posture of partners
- **Supply Chain Risk Analysis**: Identify vulnerabilities in the supply network
- **Contractual Security Requirements**: Define security obligations
- **Ongoing Monitoring**: Continuous assessment of third-party security
- **Exit Strategies**: Plan for termination of vendor relationships


# Risk Assessment Frameworks: 
`(used to identify and asses and manage risks with enterprise organization(s) and address potential threats, ensure compliance and protect asses  in operation.)`

- NIST Cybersecurity Framework (CSF): FISMA, NIST RMF (gov't issued saftey manual, emphasis on continuous monitoring and on-going risk assessment)
- ISO 27001/27005
- COSO ERM: aligns risk management w/ business strategy, designed to address risks across entire organization
- FAIR (Factor Analysis of Information Risk)
- OCTAVE (Operational Critical Threat, Asset, and Vulnerability Evaluation): tactical operations guide, analyzing from internal perspective
- COBIT (Control Objectives for Information and Related Technologies)
                        
# Risk Assessment: 
`(identifies, analyzes and evaluates risk impact and guides implementation of mitigation strategies.)`

- Quantitative analysis: Numerical data a statistical methods to measure risk
- Qualitative analysis: Subject non-numerical criteria, SME(s) experience
- Risk appetite : amount of risk org is willing to accept
- Risk tolerance: specific level of acceptable risk within appetite
- Risk prioritization: ranking of risk based on impact and likelihood
                    
# Risk Response: 
`(information and controls to mitigate identified risk)`

- Validation: confirms accuracy and completeness of identified risks
- Severity impact: quantifies consequences of validated  risk and guide prioritization
- Remediations: implementation of actionable risk management and mitigation strategies
                    
# Impact Analysis: 
`(Evaluates the consequences of identified risk on operations, asset objectives. Quantifies how adverse events could affect continuity, financial performance, and compliance.)`

- Financial impact assessment
- Operational impact assessment
- Reputational impact assessment
- Regulatory and compliance implications
- Business continuity considerations
                        