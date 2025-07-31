## Security Frameworks
Security frameworks are structured sets of guidelines, best practices, and standards designed to help organizations secure their systems, data, and operations against cyber threats.

  **Goals** : They provide a blueprint for building a strong, consistent, and compliant security posture. it provides strectured approach to implement a security lifecycle

## Security Lifecycle 

The Security Lifecycle is a cyclical process used to continuously manage and improve security in an organization. It ensures that security measures are planned, implemented, monitored, and updated to adapt to evolving threats.

## Purpose of Security Frameworks

It is used to

- **Protect PII**
- **Securing Financial info**
- **Identifying Security weaknesses**
- **Managing Organisation Risks**
- **Aligning security with business goals**

## Four Core components of framework

- **Identifying and Documenting security goals**
- **Setting guidlines to achieve security goals**
- **Implementing strong security processes**
- **Monitoring and communicating results**

**NOTE**: General Data Protection regualted by EU (GDRP). it is a data protection law established to grant European citizens more control over their personal data.

## Security Controls

Security controls are safeguards or countermeasures put in place to detect, prevent, reduce, or correct security risks. They help protect systems, networks, data, and users from threats like unauthorized access, breaches, or malware.

EX: If an organisation has all its employees to complete a training as part of complicane. As an analyst we may use a tool to auto assign and track which employees completed the tasks.

### Three Common Type of Controls:

- **Encryption** : The Process of Converting data from a  readable format to an encoded format. it is used to ensure confidentiality of sensitive data, such as customers account information (or) social security number.
- **Authentication** : It is the process of verifying, who someone (or) something is. A real-world example of authenthication is logging into a website with your username & Password.
  EX: MFA, Fingerprint, biometric
- **Authorization** : The Concept of granting access to specific resources within a system.
  
**Asset**: An item perceived as having value to an organisation.

## CIA Triad - The Foundation of Information Security

The CIA Triad is a core concept in cybersecurity that represents the three primary principles used to protect information:

 - **Confidentiality** :  Ensuring only authorized users can access sensitive data.
 - **Integrity**       :  Ensuring data is accurate, consistent, and trustworthy.
 - **Availability**    :  Ensuring data and systems are accessible when needed.


## NIST (National institue of standards and technology)

It is a U.S based agency that develops multiple voluntary compliances framework that organisations worldwide can use to help manage risk.

The more aligned an organisation is with compliance, the lower the risk.

NOTE: The guidelines and specifications can change depending on the type of organisation.

EX: Some of the framework includes

- **NIST Cybersecurity Framework (CSF)**
- **NIST Risk Management Framework (RMF)**

### NIST Cybersecurity Framework (CSF):

A voluntary framework that helps organizations manage and reduce cybersecurity risk. It’s high-level, flexible, and widely used across industries, including private and public sectors.

**Purpose** : To identify, protect, detect, respond to, and recover from cyber threats.

### The CSF consists of 6 Core Functions

- Govern
- Identify
- Protect
- Detect
- Respond
- Recover

**Goven**: Its about establishing and maintaining the structures and processes needed to Effectively manages cybersecurity risk.

**Identify** : The management of cybersecurity risk and its effect on an organizations people and assets.

**Protect** : The strategy used to protect an organisation through the implementation of policies, procedures, training and tools that help mitigate cyber security threats.

**Detect** : Identifying potential security incidents and improved monitoring capabilities to increase the speed and efficiency of detections.

**Respond** : Making sure that the proper procedures are used to contain, neutralize, and analyze security incidents, and implement improvements to the security process.

**Recover** : The Process of returning affected systems back to normal operation.


## NIST S.P.800-53:

A unified framework from protecting the security of information systems within the federal government.

### NIST Risk Management framework (RMF):

A detailed, mandatory framework (especially for U.S. federal agencies) focused on the full lifecycle of managing system security and risk — from categorization to ongoing monitoring.

**Purpose** : To help secure information systems by integrating cybersecurity, privacy, and risk management activities into the system development life cycle (SDLC).

There are seven steps in RMF
 - prepare
 - categorize
 - select
 - implement
 - assets
 - authorize
 - monitor

 **Prepare** : Activities that are necessary to manage ecurity and privacy risks before a breach occurs.
 
 **Categorize** : It is used to develop risk management processes and tasks.

 **Implement** : It is used to implement security and privacy plan for the organization.

 **Assets** : determine if establised controls are implemented correctly.

 **Authorized** : Being accountable for the security and privacy risks that may exist in an organisation.

 **Monitor** : Be aware of how systems are operating.
 
## International Organization for Standardization (ISO) :

ISO was created to establish international standards related to technology, manifactoring, and management across borders. it help organisations improve their processes and procedure for staff retention, planning, waste and services.

## Payment card industry data security standard (PCI DSS):

It is an international security standard meant to ensure that organisation store, accepts, processes and transmits credit card information can only be done in secure environment.

**Purpose** : PCI DSS Objective is to reduce credit card fraud.

  
## OWASP Security Principles:

- **Minimize Attack urface area** :  It includes all the potential vulnerabilities that a threat actor could exploit, like attack vectors.
   - Attack Vector : The pathway attacker use to penetrate security defenses.

       EX: Phishing emails & Weak passwords.
   
   - To minimise the attack Surface & avoid incidents from thi type of vectors, security teams might disable software features, restrict who can access assets (or) establish more complex password requirements.

- **Principle of least Privilege** :  Users get least amount of access to perform everyday tasks. it is to reduce the amount of damage a security breach could cause.

- **Defense in depth** : It means an org should have multiple security controls that address risks and threats in different ways.

   EX: MFA, Firewalls, intrusion detection system, and Permission settings.

- **Separation of duties** : Which can be used to prevent individuals from carrying out fraudulent (or) illegal activities.
    - This principle means that no one should be given so many privileges that they can misuse the system.

      EX: The person in a company who signs the paychecks shouldnt also be the same person who prepares them.

- **Keep security simple** : when implementing security, unnecessarily complicating solutions should be avoided because they can become unmanageable.
   - The more complex hte security controls are , the harder it is for people to work collaboratively.

- **Fix Security issues correctly** : Teck is a great tool, but can also present challenges, when a security inc occures, we are expected to identify the root cause quickly. then its important to correct any identified vulnerabilities & Conduct test to ensure that repairs are successful.

  Ex: A weak password to access an orgs wifi, as it could lead to a brach. To fix this issue, stricter password policies could be put in place.
  
### Four Additional OWASP Security
- **Establish security defaults** : it means that optimal security state of an application is also its default state for users.
  
- **Fail security** : it means that when a control fails (or) stops, it should do so by defaulting to its most secure option.
   EX: Firewall failure --> it should close all connections & block all new ones.

- **Don't trust services** : Many Organisation works with third party partners. so the organisation shouldn't explicitly trust that their partners systems are secure.

- **Avoid security by obscurity** :The Security of key systems should not rely on keeping details hidden.
