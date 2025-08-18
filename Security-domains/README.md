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

  
