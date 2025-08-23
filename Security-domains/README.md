# CISSP Eight Security Domains: (Certified information system security profession)

- **Security and Risk Management**
- **Asset Security**
- **Security Architecture and Engineering**
- **Communication and Network security**
- **Identity and access management**
- **Security Assessment and Testing**
- **Security Operations**
- **Software development security**

## Responsibilities:
- **Security and Risk Management**:

    It defines security Goals and objectives, risks mitigation, Compliance, business continuity, and the law.

    As an analyst, we may need to update policies, related to private health info, if a change is made to a federal compliance regulation such as HIPAA.

- **Asset Security**:

    It is secures digital and physical assets, it also related to the storage, maintenance, retention, and destruction of data.

    As an analyst, we may be tasked with proper disposing of old equipment and disposing of any sensitive data.

- **Security Architecture and Engineering**:

    It optimizes data security by ensuring effective tools, systems, and processes are in place.

    As an analyst, we may be tasked with configuring of firewalls.

- **Communication and Network security**:

    We manage and secure physical network and wireless communication.

    As an analyst, we may be asked to analyse user behavior in the organisation

- **Identity and access management**:

    It keeps data secure, by ensuring users follow established policies to control and manage physical assets, like office space and logical assets like networks and applications.

    As an analyst, we may be tasked with setting up employee keycard access to buildings.

  Components of IAM:
  
     - Identification : identify an user.                       EX: Username, Access card
     - Authentication : Provide Personalised verfication        EX: Password (Or) Pin
     - Authorization : Users id is confirmed, Checks if user has access to that resouce.
     - Accountability : Monitoring & Recording users actions.   EX: Logs

### Authentication:
They ask attempting to access information a simple question of "Who are you".

Factors of authentication:

   - **Knowledge** : Something the user knowns
   - **Ownership** : Something the user possesses
   - **Charateristic** : Something teh user is

**Single sign-on(SSO)**: a technology that combines several different logins into one.

**Multi-factor authentication(MFA)** : A security measure which requires a user to verifiy their identity in two (or) more ways to access a system(or) network.

### Authorization:
It is linked to the idea that access to info only lasts as long as needed.

**Seperation of duties**:
The Principle that users should not be given level of authentication that would allow them to misuse of a system. Seperating duties reduces the risk of system failures and inappropriate from users.

HTTP uses what is known as basic auth.

**Basic auth** : The technology used to establish a users request to access a server. it works by sending an identifier every time a user commuinicates with a webpage.

**OAuth** : It is an open-standard authorization protocol that shares designated access between applications, it uses API Tokens to verify access between you and a service provider.

**API token** : A small block of encrypted code that contains info about a user. these tokens contains things like the identity, site permissions, and more.

### Accounting:

It is the practice of monitoring the access logs of a system. these logs contain info like who accessed the system, and when they accessed it, what resource they used, anytime a user accesses a system, they initiate whats called a session.

**Session** : A sequence of network HTTP basic auth requests and responses associated with the same user. Two access are trigged when the session begins.
    
    - Creation of a session ID
    
    - Exchange of session cookies between a server & users device.

**Session ID** : It is a unique token that identifies a user and their device while accessing the system.

**Session Cookies** : It is a token that websites user to validate a session and determine how long that session should last. cookies make websessions safer and more efficient.

**Session Hijacking** : It is an attacker can impersonate a user their session token. this is called session hijacking. It is an event where attackers obtain a legitimate user's session ID.

- **Security Assessment and Testing**:

   Conducting security control testing, collecting and analyzing data, and conducting security audits to monitor for risks, threats and vulnerabilities.

    As an analyst, we may conduct regular audits of users permissions, to make sure that users have the correct level of access.

- **Security Operations**:

  Conducting Investigations and implementing presention measures.

  As an analyst, we may need to follow organisations policies and procedures to quickly stop the potential threats.

- **Software development security**:

  Uses security coding practices, which are a set of recommended guidelines that are used to create secure application and services.

  As an analyst, we may work with software development teams to ensure security practices are incorporated into the software development life cycle.


## User Provisioning :
It is the process of creating and maintaining a users digital identity.

**Granting Authorization**:
There are three common frameworks that orgs use to handle there IAM steps.

- Mandatory access control (MAC)
- Discretionary access control (DAC)
- Role-based Access control (RBAC)

### Mandatory Access Control (MAC):
It is the strictest of the three framework. Authorization is strict need to know basis. Access to info must be granted manually by a central authority (or) system.

### Discretionary Access Control (DAC) :
It is typically applied where a data owner decides appropriate level of access.

### Role Based Access Control (RBAC) :
It is used when authorization is determined by a users role within an organization.

## Common Vulnerabilities & Exposures list (CVE list) :
It is an openly accessibile dictionary of known vulnerabilities and exposures. it was originaly created by MITRE Corp.

### MITRE :
It is a collection of non-profile research and development centres sponcered by US Government.

### CVE Numbering Authority(CNA):
It is an organization that volunters to analyze and distribute information on eligible CVEs.

**CVE list Criteria** :
- Independent of other issues
- Recognized as a potential security risk
- Submitted with supporting evidence
- Only affect one codebase.

### Common vulnerability scoring system (CVSS) -(0-10)
It is a measurement system that scores the severity of a vulnerability. this is a way of calculating the impact a vulnerability could have on a system. They also use them to determine how quick it should be patched.

### Open Source intelligence (OSINT) :
It is the collection and analysis of information from publicly available sources to generate usable intelligence. it plays a significant role in information security(info sec), which is the practice of keeping data in all states away from unauthorized users.

**Ways OSINT can be used to generate instelligence** :
- Provide insights into cyber attacks
- To detect potential data exposures
- To evaluate existing defenses
- To identify unknown vulnerabilities

## PASTA (The Process for attack simulation and threat analysis) :

**Attack Tree** : It is a diagram that maps threats to assets.

It is a popular threat modeling framework thats used across many industries. Stages of this framework are

1) Define business and Security objective
2) Define the technical Scope
3) Decompose the application
4) Perform a threat analysis
5) Perform a Vulnerability analysis
6) Conduct attack modeling
7) Analyze risk & Impact

The Security team uses attack trees to identify attack vectors. 

           Ex:  |__Customer info Database__|        |__Customer info DB__|          |__Customer info DB__|
                            |                                 |                               |
                                                      |__SQL Injection__|            |__SQL injection__|
                                                                                              |
                                                                                    |__Unsanitized inputs__|
Some of the other common frameworks are

## Common frameworks :

When performing threat modeling there are multiple methods that can be used such as

- **STRIDE** : It is a threat - modeling framework developed by microsoft. it commonly used to identify vulnerability in 6 attack vectors.

  1) Spoofing
  2) Tampering
  3) Repudiation
  4) Information disclosure
  5) Denial of service
  6) Elevation of Privilege    
  
- **Trike** : It is an open source methodology and tool that takes a security centric approach to threat modeling.
  
- **VAST** : The Visual, Agile, and simple threat (VAST) modeling framework is part of an automated threat modeling platform called Threat modeler.

