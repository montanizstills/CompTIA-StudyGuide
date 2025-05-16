# Attack Surface Management and Reduction

## Vulnerability Management
- **Definition**: Systematic process of identifying, evaluating, treating, and reporting on security vulnerabilities in systems and software.
- **Key Components**:
  - Asset inventory (complete visibility of all assets)
  - Vulnerability scanning (routine and automated)
  - Risk assessment and prioritization
  - Patch management
  - Remediation workflows and verification
- **Critical Metrics**:
  - Mean time to remediate (MTTR)
  - Vulnerability density
  - Patch coverage percentage
  - Risk reduction over time
- **Best Practices**:
  - Implement risk-based approach for prioritization
  - Maintain comprehensive vulnerability database
  - Establish clear remediation SLAs
  - Document exceptions with compensating controls

## Hardening
- **Definition**: Process of securing a system by reducing its attack surface and eliminating potential attack vectors.
- **System Hardening Techniques**:
  - Remove/disable unnecessary services, ports, accounts
  - Apply security patches promptly
  - Implement principle of least privilege
  - Configure secure authentication mechanisms
  - Remove default/sample files
- **OS Hardening**:
  - Follow CIS benchmarks for configuration
  - Disable unnecessary system services
  - Enable host-based firewalls
  - Implement application whitelisting
  - Deploy EDR solutions
- **Network Hardening**:
  - Segment networks with proper zoning
  - Implement 802.1x for network access control
  - Use VLANs for traffic isolation
  - Deploy IDS/IPS systems
  - Implement zero trust principles

## Defense-in-Depth
- **Definition**: Layered security approach that employs multiple defensive mechanisms to protect valuable data and information.
- **Key Layers**:
  - Physical (facility access controls, CCTV)
  - Network (firewalls, IDS/IPS, segmentation)
  - Host (antimalware, host firewall, EDR)
  - Application (SAST/DAST, WAF, secure coding)
  - Data (encryption, DLP, access controls)
- **Implementation Guidelines**:
  - Ensure controls at each layer work independently
  - Implement both preventative and detective controls
  - Design overlapping protection mechanisms
  - Consider both internal and external threats
  - Establish recovery capabilities

## Legacy Components within an Architecture
- **Challenges**:
  - Outdated/unsupported systems
  - Limited/no security updates
  - Integration vulnerabilities
  - Non-compliance with modern security standards
- **Mitigation Strategies**:
  - Isolation/containment (network segmentation)
  - Implement compensating controls
  - Virtual patching with WAF/IPS
  - Strict access control policies
  - Enhanced monitoring and logging
  - Develop migration/replacement roadmap
- **Risk Assessment Considerations**:
  - Business impact of compromise
  - Exposure to critical data/systems
  - Regulatory compliance implications
  - Operational dependencies

# Detection and Threat-Hunting Enablers

## Centralized Logging
- **Purpose**: Aggregation of log data from multiple sources for comprehensive analysis and correlation.
- **Components**:
  - Log collectors/forwarders
  - Central log repository/SIEM
  - Log parsing and normalization engines
  - Retention and archiving capabilities
- **Critical Log Sources**:
  - Network devices (firewalls, routers, switches)
  - Security devices (IDS/IPS, WAF, proxies)
  - Authentication systems
  - Operating systems
  - Applications and databases
  - Cloud services and infrastructure
- **Implementation Best Practices**:
  - Establish baselines for normal behavior
  - Implement secure log transmission
  - Define appropriate retention periods
  - Ensure time synchronization (NTP)
  - Protect log integrity and confidentiality

## Continuous Monitoring
- **Definition**: Ongoing awareness of information security vulnerabilities and threats to support risk management decisions.
- **Key Elements**:
  - Real-time visibility across environment
  - Automated data collection and analysis
  - Behavioral baseline establishment
  - Anomaly detection capabilities
  - Integration with threat intelligence
- **Monitoring Categories**:
  - Network traffic monitoring
  - User behavior analysis
  - Configuration and compliance monitoring
  - Vulnerability and patch monitoring
  - Asset discovery and inventory
- **Implementation Approach**:
  - Define critical assets and monitoring priorities
  - Establish performance baselines
  - Automate data collection where possible
  - Determine appropriate monitoring frequency
  - Document monitoring requirements

## Alerting
- **Purpose**: Notification system to inform security teams of potential security incidents or anomalies.
- **Alert Types**:
  - Signature-based (known threat patterns)
  - Behavioral (deviations from baselines)
  - Threshold-based (exceeding predefined limits)
  - Correlation-based (multiple events indicating attack)
- **Alert Management**:
  - Prioritization frameworks (severity, impact)
  - Alert enrichment processes
  - Alert routing/escalation procedures
  - False positive reduction mechanisms
  - Alert lifecycle tracking
- **Best Practices**:
  - Define clear alert thresholds
  - Implement tiered alerting structure
  - Establish alert response workflows
  - Regularly review and tune alert rules
  - Measure and improve alert quality

## Sensor Placement
- **Definition**: Strategic positioning of security monitoring tools to maximize visibility and detection capabilities.
- **Sensor Types**:
  - Network-based (taps, SPAN ports)
  - Host-based (agents, collectors)
  - Application-based (API integrations)
  - Cloud-based (VPC flow logs, CASB)
  - Physical (cameras, access systems)
- **Placement Considerations**:
  - Network choke points and boundaries
  - Critical asset proximity
  - Visibility requirements (north-south vs. east-west)
  - Performance impact
  - Regulatory compliance needs
- **Coverage Areas**:
  - Internet gateways
  - Inter-VLAN routing points
  - Data center interconnects
  - Cloud-to-on-premise connections
  - Critical server segments
  - User access points

# Information and Data Securing Design

## Classification Model
- **Purpose**: Framework for categorizing data based on sensitivity and organizational value.
- **Common Classification Levels**:
  - Public (non-sensitive, freely shareable)
  - Internal (business use, limited distribution)
  - Confidential (sensitive, restricted access)
  - Restricted/Highly Confidential (critical, strictly controlled)
- **Implementation Steps**:
  - Define classification criteria
  - Document classification policy
  - Train users on classification procedures
  - Implement supporting technical controls
  - Establish audit and review processes
- **Considerations**:
  - Regulatory requirements
  - Business impact of unauthorized disclosure
  - Industry-specific classifications
  - Partner/third-party requirements
  - Reclassification procedures

## Data Labeling
- **Definition**: Process of applying visual or metadata identifiers to data assets indicating their classification.
- **Labeling Methods**:
  - Visual markings (headers/footers, watermarks)
  - Metadata tagging
  - Electronic file/document properties
  - Container-level labeling (databases, shares)
- **Implementation Approaches**:
  - Manual labeling by users
  - Automated content inspection
  - Default labeling based on location/source
  - Hybrid approaches
- **Best Practices**:
  - Consistent labeling format and terminology
  - User-friendly labeling interfaces
  - Automated validation where possible
  - Regular compliance auditing
  - Integrated with DLP systems

## Tagging Strategies
- **Purpose**: Systematic approach to applying metadata to data assets for security, governance, and management.
- **Tag Types**:
  - Classification tags (sensitivity level)
  - Compliance tags (regulatory frameworks)
  - Retention tags (lifecycle management)
  - Ownership tags (responsible entities)
  - Purpose tags (usage restrictions)
- **Implementation Methods**:
  - Schema-based tagging frameworks
  - Automated tagging based on content
  - User-driven tagging with validation
  - Inheritance-based tagging
- **Best Practices**:
  - Develop standardized tag taxonomy
  - Implement tag governance processes
  - Ensure tag propagation across systems
  - Integrate with access control mechanisms
  - Regularly audit and validate tag accuracy

# DLP (Data Loss Prevention)

## At Rest
- **Definition**: Protections for data stored on endpoints, servers, databases, and storage systems.
- **Key Technologies**:
  - Content discovery and classification
  - File system monitoring
  - Database activity monitoring
  - Encryption (FDE, file-level, transparent)
  - Access control mechanisms
- **Implementation Approaches**:
  - Automated scanning and discovery
  - Policy-based access restrictions
  - Rights management integration
  - Secure deletion mechanisms
  - Data masking technologies
- **Best Practices**:
  - Focus on high-value data repositories
  - Implement least privilege for data access
  - Conduct regular data discovery scans
  - Encrypt sensitive data appropriately
  - Monitor unauthorized access attempts

## In Transit
- **Definition**: Protections for data moving across networks, between systems, or to/from endpoints.
- **Key Technologies**:
  - Transport encryption (TLS/SSL)
  - Email DLP (content filtering, encryption)
  - Secure file transfer protocols
  - Web gateway filtering
  - CASB for cloud data transfers
- **Control Types**:
  - Preventative (blocking unauthorized transfers)
  - Detective (identifying policy violations)
  - Corrective (encrypting/redirecting transfers)
- **Implementation Considerations**:
  - Network traffic inspection points
  - Encrypted traffic analysis
  - Performance impact
  - Mobile device coverage
  - Cloud service integration

## Data Discovery
- **Purpose**: Process of identifying and locating sensitive data across the enterprise environment.
- **Discovery Methods**:
  - Pattern matching (regex, keywords)
  - Fingerprinting/exact data matching
  - Machine learning classification
  - Context-based identification
  - Metadata analysis
- **Discovery Scope**:
  - Structured repositories (databases)
  - Unstructured data (documents, images)
  - Semi-structured data (email, messaging)
  - Endpoint storage (laptops, mobile)
  - Cloud storage (SaaS, IaaS)
- **Best Practices**:
  - Prioritize high-risk environments
  - Establish discovery cadence
  - Validate findings with sampling
  - Document discovery coverage
  - Integrate with remediation workflows

# Third-Party Integrations
- **Security Considerations**:
  - API security (authentication, authorization)
  - Data transmission security
  - Access control mechanisms
  - Audit and logging capabilities
  - Vulnerability management process
- **Integration Models**:
  - Point-to-point integrations
  - Hub-and-spoke architectures
  - Enterprise service bus
  - API gateway models
  - Microservices integrations
- **Risk Management Approaches**:
  - Vendor security assessment
  - Integration security testing
  - Data flow mapping and analysis
  - Contractual security requirements
  - Ongoing monitoring and review
- **Best Practices**:
  - Implement least privilege access
  - Encrypt sensitive data exchanges
  - Validate input/output at integration points
  - Implement robust authentication
  - Establish comprehensive logging

# Control Effectiveness

## Assessments
- **Types of Assessments**:
  - Security control assessments
  - Risk assessments
  - Gap analysis
  - Compliance assessments
  - Penetration testing
- **Assessment Methodologies**:
  - Interview-based assessment
  - Documentation review
  - Technical validation/testing
  - Observation of processes
  - Tabletop exercises
- **Assessment Frequency**:
  - Periodic (annual, quarterly)
  - Continuous assessment
  - Event-driven (post-incident, major changes)
  - Risk-based (higher risk = higher frequency)
- **Best Practices**:
  - Define clear assessment scope and objectives
  - Use standardized assessment frameworks
  - Ensure appropriate subject matter expertise
  - Document and track findings systematically
  - Integrate with remediation processes

## Scanning
- **Scanning Types**:
  - Vulnerability scanning
  - Configuration compliance scanning
  - Network discovery scanning
  - Web application scanning
  - Database scanning
  - Container/image scanning
- **Scanning Approaches**:
  - Authenticated vs. unauthenticated
  - Agent-based vs. agentless
  - Internal vs. external perspective
  - Manual vs. automated
- **Scanning Frequency**:
  - Continuous monitoring
  - Scheduled periodic scans
  - Event-driven scanning
  - Risk-based frequency adjustment
- **Best Practices**:
  - Minimize operational impact
  - Validate scanning coverage
  - Tune scanning for false positive reduction
  - Integrate with change management
  - Establish clear scan ownership

## Metrics
- **Key Security Metrics Categories**:
  - Vulnerability management metrics
  - Incident response metrics
  - Compliance metrics
  - Operational security metrics
  - Risk management metrics
- **Effectiveness Metrics Examples**:
  - Mean time to detect (MTTD)
  - Mean time to remediate (MTTR)
  - Coverage metrics (asset, control, patch)
  - False positive/negative rates
  - Risk reduction over time
- **Metric Development Process**:
  - Define measurement objectives
  - Identify key performance indicators
  - Establish data collection methods
  - Determine calculation methodologies
  - Set performance targets/thresholds
- **Best Practices**:
  - Focus on actionable metrics
  - Ensure metric reliability and consistency
  - Develop balanced metric sets
  - Establish regular reporting cadence
  - Review and refine metrics periodically