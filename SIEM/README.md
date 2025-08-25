# SIEM (Security Information and event management) Tools
it is an application that collects and analyzes log data to monitor critical activities in an organisation. It provides real-time visibility, event monitoring and analysis, and automated alerts. it also stores all log data in a centralized location. SIEM tools index and minimize the number of logs a security professional must manually review and analyze, they increase efficiency and save time.

## SIEM Dashboards
It helps security analysts quickly and easily access their org's security information as charts,graphs, (or) tables. SIEM dashboards provide stakeholder with metrics.

### Metrics
They are key Technical attributes, such as response time, availability, and failure rate, which are used to assess the performance of a software application 

## Different type of SEIM tools

- **Self-hosted**: This SIAM Tools Require Organisations to install operate, and maintain the tools using their own physical infra, such as servers capacity. They are managed and maintained by orgs IT department rather than third party vendor. They are ideal if an orgs needs physical control over confidential data.

- **Cloud-hosted** : They are managed by SIEM Providers. They are prefered if we dont want to invest in creating and maintaining their own infrastrecture.

- **Hybride** : Organisations can choose to use a combination of both self hosted and cloud hosted SEIM tools, It is called hybrid solution.

  
SIEM Tools collect data real time and allows analysts to identify security breaches as they happen.
Commonly used SIEM Tools are
   
  - **Splunk Enterprise**
  - **Splunk Cloud**
  - **Chronicle**

Other key security tools include
   
  - **Playbooks**
  - **Network Protocol analyzers**

**Playbook**: A manual that provides details about any operational action. They Vary from one organisation to the next, guide analysts in how to handle a security incident before, during and after it has occured.Playbooks can pertain to security (Or) Compliance review, Access management, and many other Organizational tasks that requrie Documented process from beginning to end.

**Network Protocol analyzers(Packet Sniffer)** : A tool designed to Capture and analyze data traffic within a network. Common packet Sniffers include TCP dump and wire sharks.

**Programming** : It is used to create a specific set of instructions for a computer to execute tasks.

**Structured Query Language(SQL)** : A Programming Language used to create interact with, and request information from a database.

## Logs : 

It is a recoed of events that occure within an organization systems and networks.

The Common log sources are
   - Firewall logs
   - Network logs
   - Server Logs

**Firewall logs** : It is a record of attemped (or) established connections for incoming traffic from the internet. it also includes outbound requests to the internet from within the network.

**Network logs** : It is a record of all computers and devices that enter and leave the network. it also records connections between devices and services on the network.

**Service logs** : it is a record of events related to services, such as website, email (or) file shared. includes actions such as login, password, and username requests.

## Playbook :
It is a manual that provides details about any operational action. They also clarity what tools should be used in response to a security incident. Playbooks ensure that People follow a consistent list of actions in a prescribed way. Regardless of who is working on the case different types of playbook are used.

These includes playbook for incident response security alerts, Team-specific, and product specific purposes.

## Incident response playbooks:

An Organizations quick attempt to identify an attack , contain the damage, and correct the effects of a security breach. It is a guide with 6 phases used to help mitigate & manage Security incidents from beginning to end.

## Virus Total:

It is a database tool that has hash values of known online viruses. people use this for analyzing suspicious files, domains, IPs, and URLs.

## Intrusion detection system (IDS) :

It is an application that monitors system activity and alerts on possible intrusion.

## Detection Tool Types :

- Detection and management tools
- Documentation tools
- Investigative tools

**Documentation** : It is any form of recorded contents that is used for a specific purpose.

### Types of Documentation :

  - Playbook
  - Incident handler's Journals 
  - Policies
  - Plans
  - Final Reports
    
There are no industry standard for documentation.

### Intrusion detection system (IDS) :

It is an appliation that monitors system and network activity and produces alerts on possible intrusions.

### Intrusion Prevention system (IPS) :

It is an application that monitors system activity for intrusions and take action to stop the activity.

### IDS and IPS tools :

  - Snort
  - Zeek
  - Kismet
  - Sagan
  - Suricata

### Endpoint detection and response (EDS) :

EDS is an application that monitors an endpoint for malicious activity. EDR tools are installed on endpoints. endpoint is any device connected to a network.

## Security Information and Event Management (SIEM) :

An application that collects and analyzes log data to monitor critical activities in an organization.

### SIEM Process :

1) Collect and aggregate date (mostly logs)
2) Normalize data
3) Analyze data

**Security Orchestration, automation, and response (SOAR)** :
A Collection of applications, Tools, and work flows that uses automation to respond to security events.

**Network Traffic** : The amount of data that moves across a network.

**Network data** : It is the data thats transmitted between devices on a network.

## Indicators of compromise (IOC) :

Observable evidence that suggestes signs of a potential security incident. we can think of data exfiltration.

**Data Exfiltration** :

Unauthorized transmission of data from a system. They are used to Steal (or) leak data such as user name, Password (or) Intellectual Property.

**Command and Control (C2)**:

It is when malicious actors use protocols and Ports that are not commonly associated to maintain communications between the compromised system and their own machine.

**Packet Payload information**:

It is the actual data thats transmitted in network Packets often, This data is encrypted and requires decryption for it to be readable.

**Temporal Patterns** :

Network Packets Contain information relating to time. This information is useful in understanding time Patterns. if large volumes of traffic are suddenly outside of the normal hows of network activity, then this is considered off basline and should be investigated.

### Defensive Measures for Exfiltration attacks:

  1) Prevent attacker access
  2) Monitor Network activity
  3) Protect assets
  4) Detect and Stop the exfiltration

### Lateral Movement : (or) (Pivoting) :

It describes an attacker exploring a network with the goal of expanding and maintaining their access.

### Network Protocol Analyzer : (or) (Packet Sniffer) 

It is a tool desined to capture and analyze data traffic within a network.

## Packet Capture (P-Cap) :

A file Containing data packets intercepted from an interface (or) network. P-Cap Files can come in many formats depending on the packet capture library. some of the libraries & Formats are 

1) **LibPCap** : It is a Packet capture library designed to be used by unix-like system, like linux & macOS. Tools like tcpdump use LibPcap as the default Packet Capture.
2) **WinPcap** : It is an Open-Source Packet Capture library designed for devices running windows OS. its an old file format & isn't mainly used.

3) **NPCap** : It is a library designed by the Port Scanning tool Nmap that is commonly used in windows OS.

4) **PCAPng** : It is a modern file format that can simultaneously capture packets and store data. Its ability to do both explains the "ng", which Stands for "next generation".

