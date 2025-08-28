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
