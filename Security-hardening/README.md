# Security Hardening

It refers to the process of reducing vulnerabilities in systems like networks, cloud environments, servers, and applications—to protect them from threats, attacks, and unauthorized access.

## Network Security hardening

It focuses on network related security hardening like

  - Port Filtering
  - Network access privilege
  - Encryption

Some network hardening tasks are performed regulated while some are performed once and updated overtime. some common tasks performed are

  - Firewall rules maintenance
  - Network Log analysis
  - Patch updates
  - Server backups

### Network Log Analysis

It is the process of examining network logs to identify events of interest. security teams use a log analyzer tool (or) security information and event management tool (SIEM), to conduct network log analysis

**Port Filtering** : it is a firewall funtion that blocks (or) allows certain port numbers to limit unwanted communication.

### Intrusion detection system (IDS) :

An IDS is an application that monitors systems activity and alerts on possible intrusion. An IDS alerts admins based on the signature of malicious traffic. It is configured to detect known attacks.
They sniff data packets as they move across the analyze for the characteristics of known attacks.

The Limitation of IDS systems are that they can only scan for known attacks. New and Sophisticated attacks might not be caught. They can also not stop any incoming traffic even if it detects something.

### Intrusion Prevention system (IPS) :

An IPS is a system that monitor system activity for intrusive activity and takes action to stop the activity. It offers more protection then an IDS as it can actively stop anomalies when they are detected.

The Limitation is that it is inline is if it breaks, the connection between the private network and the internet breaks. it can also give false positives, which can result in legitimate traffic dropped.

### Full Packet Capture devices :

They can allow us to record and analyze all of the data that is transmitted over our network. they can also help in investigating alerts created by an IDS.

### Cloud Network :

A Collection of servers (OR) Computers that Stores resources and data in remote data centers that can be accessed via the internet. One different between cloud network hardening and traditional network hardening is the use of a server baseline image for all server instance stored in the cloud

### Zero day attacks :

They are an important security consideration for Organisation using cloud (or) traditional on-premise network solution. A Zero day attack is an exploit that was previously unknown. Cloud providers are more likely to know about a zero day attack occurring before a tradition IT organisation.

## Cloud Security Hardening :

There are various Techniques and tools that can be used to Secure Cloud network infrastruture and resources. Some of the Common CSH Techniques include IAM, hypervison baselining, cryptography, and cryptographic erasure.

### Identity access management (IAM):

IAM is a collection of processes and technologies that helps organizations manage digital identities in their env. This service also authorizes how users can leverage different cloud resources.

### Hyper Visors:

A hypervisor abstracts the hosts hardware from the OS environment. hypervisors are two types

  - Hypervisors that run on the hardware of the host PC.
  - Hypervisors that runs on the software of the host PC.

### Baselining :
 It Cover how the cloud environment is configured and set up it is a fixed reference point, and this can be used to compare changes made to a cloud environment.

 Proper configureation and setup can greatly improve the security and performance of a cloud env.

 EX: 1) Restricting access to the admin portal
     2) enable password management
     3) enable file encryption
     4) enabling threat detection for SQL database.

### Cryptography :

It can be applied to security data that is processed and stored in a cloud env. cryptography encription is a key way to secure sensitive data. crytography uses encryption and secure key management system to provide data integrity and confidentiality.

### Cryptographic Erasure :

It is a menthod of erasing the encryption key for the encrypted data. when destroying data in the cloud, more traditional menthods of data destruction are not as effective.

### Crypto-shredding :

It is a new technique where the cryptographic keys used for decryption the data are destroyed. this makes data undecipherable. All copies of the key need to be destroyed so no one has any opportunity to access the data in the future.
