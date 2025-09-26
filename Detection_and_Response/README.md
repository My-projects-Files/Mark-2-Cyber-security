# Practical

## Punycode: 
It is a part of DNS resolution where It is used to converting words that cannot be written in ASCII, into a unicode ASCII encoding. The original DNS only supports ASCII, so we can't use domains 

    ex: münchen.de, café.com

To support (IDNS) international Domain names, we need a way to convert unicode to ASCII. so for unique domains like above, we can use

      münchen.de   ----->  xn--mnchen-3ya.de

now wen we enter a unicode domain, the browser converts it to punycode before querying DNS. its also used in email system,SSL Cert, Web servers.

### Security Risk of punycode:

They can be abused for phishing, using visually similar char like

    apple.com ---> app1e.com (cgrillic letters)



# NIST CSF:

The Five Core funtions of the NIST CSF are identify, protect, detect, respond, and recover. the last three steps called detect, respond, and recover are critical stages during incident response. the NIST incident response lifecycle is another NIST framework with steps dedicated to incident response.

1) Prepation
2) Detection and analysis
3) Containment Eradication
4) Recovery
5) Post Incident activity

its not a linear process, so steps can overlap as new discovers are made.

## Incident :
It is an occurence that actually (or) imminently jeopardizes, without lawful authority, the confidentiality, integrity, (or) availability of information (or) an information system, (or) Constitutes a violation (or) imminent threat of violation of law, security policies, Security procedures, (or) acceptable use policies.

**NOTE**:  All Security incidents are events, but not all events are security incidents.

**Event** : An Observable Occurrence on a network, system, (or) device.

### The 5 W's of an incident

  - Who Triggered the incident
  - What happened
  - When the incident took place
  - Where the incident took place
  - Why the incident Occured

### Incident handler's journal : 
It is a form of documentation used in incident response.

## Computer Security incident responce teams (CSIRT) :

A Specialized group of security professionals that are trained in incident management and response. The goal of CSIRT are to effectively and efficiently manage incidents, Provide Services and resources for response and recovery, and to prevent future incidents.

### Roles in CSIRT :

  - Security analyst --> They investigate security alerts to determine if an inc has occured
  - Technical lead --> They Provides Technical leadership by guiding security Incident through their lifecycle.
  - Incident Coordinator --> They tracks and manages the activities of the CSIRT & other teams Involved in the response effort.

## Security operations Center (SOC) :

It is organizational unit dedicated to monitoring network, system, and devices for security threats (or) attacks.

### SOC Organization :
It is composed of SOC analysts, SOC leads, and SOC managers.

**Tier 1 SOC Analyst** : It Composed of the least experienced SOC analysts who are known as Level 1. They usually do monitoring, reviewing, and prioritizing alerts, Creating & Closing alerts ticket system etc.

**Tier 2 SOC Analyst** : It composed of more experienced SOC analysts, they are responsible for receiving escalated tickets from L1 and configuring, refining security tools, and reporting to Lead.

**Tier 3 SOC Lead** : It Composed of the SOC Leads, managing team operations, exploring methods of detection by performing advanced detection techniques, such as malware & forensics analysis. they report to SOC manager.

**SOC manager** : He is at the top and is responsible for hiring , Training,and evaluating the SOC team members. Creating and managing the Performance of the SOC team. Developing reports, Communicating with stake holders.

## Incident Response Plan :
It is a document that outlines the Procedures to take in each step of incident response. Organizations tailor their plans to meet their unique requirements such as their mission, size, culture, industry and structure.

### Most common elements of an incident Plan:

  - Incident Response Procedures --> Step-by-Step instructions
  - System information --> Network diagram , data flow diagram, logging.
  - Other documents --> Like contact lists, Forms, & Templates.


## Detection :

It is the Prompt discovery of Security events. 

**Note** : Not all events are incidents, But all incidents are events.

### Analysis :

It involves the investigation and validation of alets.

Challenges in the detection and analysis Phase.

  - Impossible to detect everything
  - High volumes of alerts

## Threat hunting :

It is a proactive search for threats on a networks. we use them to uncover malicious activity that was not identified by detection tools and as a way to do further analysis on detections. it is also used to detect threats before they cause damage.

### Threat hunters :

They are specialists in threats hunting. They perform research on emerging threats and attacks and then determine the Probability of an organization being vulnerable to a paticular attack.

They use a combination of threat intelligence, indicatiors of compromise indication of attack, and ML to search for threats.

### Threat intelligence :

It is an evidence - based threat information that provides context about existing (or) emerging threats.

Threat intelligence can come from private (or) public source like

  - **Industry reports** --> Includes details about attackers tactics, techniques, and Procedures (TTP).
  - **Government advisories** --> Similar to industry reports, government advisories include (TTP).
  - **Threat data feeds** --> It Provide a stream of threat-related data that can be used to help protect against sophisticated attackers like advanced persistent threats (APT).

### Advance Persistent threats (APT) :
They are instances when a threat actor maintains unauthorized access to a system for an extended Period of time. The data is usually a list of indicators like IP addresses, domains, and file hashes.

### Threat Intelligence Platform (TIP) :

It is an application that collects, centralizers, and analyzes threat intelligence from different sources.

### Cyber deception :

It involves techniques that deliberately deceive malicious actors with the goal of increasing detection and improving defensive strategies.

### Honey Pots:

They are an example of an active cyber defense mechanism that uses deception technology. they are systems (or) Resources that are created as decoys vulnerable to attacks with the purpose of attracting potential intruders.

## Automation for finding Threats:

CI/CD Pipelines help release software faster, but they can also open up new vulnerabilities for attackers. when these threats are found, seurity teams can response quickly and limit the damage. this automated threat detection is a main goal of strong CI/CD security.

### Common Indicators of Compromise (IOC) in CI/CD Pipelines :

By understanding common IOC in CI/CD helps us monitor effectively and quickly find security incidents.

  - **Unauthorized code changes** --> Code changes from people who shouldn't be making changes and chnages made at unusual times (or) from unexpented locations also changes that look suspicious, like confusing code, very large deletions without a good reasons, (or) code that dont follow coding rules.
  
  - **Suspicious Deployment patterns** --> Deployments to unusual (or) unapproved system, and deployment happening at unexpected times (or) too often, and they started by unusual accounts (or) automated accounts that should not be releasing to prod.

  - **Compromised Dependencies** --> Finding known vulnerabilities (CVEs) independencies during automated checks in the CI/CD pipelines. suddenly adding new, unexpected dependencies to build settings. attempts to download dependencies from unofficial (or) untrusted sources.

  - **Unusual Pipeline execution** --> Pipeline steps that normally works suddenly fails. they taking much longer to run for no clear reason and changes being made.

  - **Secrets exposure attempts** --> logs showing atteptsto get to secrets from unapproved places in pipeline. finding Private secrets hardcoded in code changes.

### Proactive security through monitoring for IOC :

ongoing monitoring of CI/CD pipelines, focusing on anomaly detection and finding IOCs, Making our security stronger and more Proactive by using monitoring tools we can prevent damage by

  - Respond to incidents quickly
  - Limit the damage
  - Improve threat knowledge

## Using Automation to find anomalies & IOCs:
we can use this methods, for monitor CI/CD Pipelines & automatically find threats.

  1) **Comprehensive logging and auditing** : Detailed logs are bases of monitoring. logs provide the raw data that monitoring tools check for unusual activity and Potential indicators of Compromise (IOC). The most common logs for finding anomalies are

     - Pipeline Execution logs
     - Code commit logs
     - Access Logs
     - Deployment logs
    
  2) **Security information and event management (SIEM) integration** : Connecting our CI/CD logs to a SIEM tool can help automatically find anomalies at a large scale. SIEM Platforms are made

      - Automatically find anomalies
      - Use Rules to alerts for known IOC's

  3) **Real-time Alerting and Notifications** : Automated alerts make sure Security teams are notified right away about unusual activity and possible IOC's, so they can respond quickly. Alerts should be setup for :

      - Unusual Build Failures
      - Suspicious code changes (Based on Anomalies)
      - Attempts to expose secrets
      - Unusual Network Traffic
  4) **Performance Monitoring to find IOA's and discover IOC's** : It is mainly used to make sure things are running smoothly, can also indirectly help find IOC's. Performance issues (indicators of attack - IOAs) like sudden slowdowns (or) CI/CD servers running out of resources can lead to deeper checks that may uncover IOC's.

  5) **Continuous Vulnerability Scanning** : Regularly checking the CI/CD infra for weaknesses can proactively find vulnerable parts. This includes common vulnerabilities and exposures (CVEs) in CI/CD tools, Plugins, and containers. they are potential IOC's.

### Indicators of compromise (IOC's) :

They are observable evidence that suggests signs of a Potential security incident. IOC's chart specific Pieces of evidence that are associated with an attack, like file name associate with a type of malware.

### Indicators of attack (IOA) :

They are the series of observed events that indicate a real-time incident. IOA's focus on identifying the behavioral evidence of an attacker, including their methods and intentions.

indicators of compromise are not always a confirmation that a security inc has happened. IOC may be the result of human error, system malfunctions, and other reasons not related to security.

**NOTE**: IOC's help of identify the who and what of an attack after its taken place, while IOA's focus on finding the way and how of an ongoing (or) unknown attack.

## Pyramid of pain:

Not all IOC's are equal in the value they provide to security teams. They Pyramid of pain Captures the relationship between IOC's and the level of difficulty that malicioius actors experience when indicators of compromise are blocked by security teams.

Each type of IOC's is seperated into level of difficult. these represents the "pain" level that an attacker faces when security teams blocks the activity associated with the indicator of compromise.

                    /   \
                  /__TTPs__\
                 /__Tools___\ 
                /Network/Host\
               /__Artifactos__\ 
              /__domain Names__\
             /__IP addresses____\
            /____Hash__Values____\ 

## Benefita of documentation:

  - Transparency
  - Standardization
  - Clarity

### Chain of custody:
The Process of documenting evidence Possession and control during an incident lifecycle.

**Broken Chain of Custody**: Inconsistencies in the collection and logging of evidence in the chain of custody.

**Chain of Custody establishes**

  - Integrity
  - Reliability
  - Accuracy


### Type of Playbook:

  1) Non-automated ---> Step-by-step actions Performed by an analyst
  2) Automated ---> It automate tasks in incident response processes
  3) Semi-Automated ---> It combines a Persons action with automation.

Semi-automated Playbooks can help increase Productivity and decreaser time to Resolution.

# Triage

The Prioritizing of incidents according to their level of importance (or) Urgency.

## Processes of Triage:

  1) Receive and assess
  2) Assign Priority
  3) Collect and analyze

**Questions to ask**:

  - is there anything out of the ordinary ?
  - Are there Multiple failed login attempts ?
  - Did the login happen outside of normal working hours ?
  - Did the login happen outside of the network ?

### Assign Priority :
Once an alert has been properly assesses and verified as a security issue, it needs to be prioritized accordingly, Incidents differ in their impact, Size, and Scope, which affests the response efforts.

### Factors to Consider when setting priority:

- **Functional Impact** : Security incidents that target information technology systems impact the service that these systems provide to its users. consider how INC the business funtionality of affected system.
  
- **Information Impact** : Incidents can affect the confidentiality, integrity, and availability of an organization's data and information. Consider the effects that information compromise can have beyond the organization.
  
- **Recoverability** : How an Org Recovers from an incident depends on the size and scope of the incident and the amount of resources available. consider whether recovery is possible and consider whether it's worth the time and cost.

## Benifits of Triage :

By Prioritizing incs based on their potential impact, we can reduce the scope of impaact to the Organization by ensuring a timely response. here are some benifits.

  - **Resource Management** : Triaging alerts allows security teams to focus their resources on threats that require urgent attention.
  - **Standardizing approach** : Triage Provides a standardized approach to incident handling. process documents, like playbooks help to move alerts through an iterative proccess to ensure that alerts are properly assessed & Validated.
