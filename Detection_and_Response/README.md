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

They are specialists in threats  
