# Assets, Threats ,and Vulnerabilities

**Risk** : Anything that can impact the Confidentiality, integrity, (or) availability of an assets.

## Security risk planning

They are based on the analysis of three elements. They represents what, why, and how of security.

  - **Assets** : It is an item perceived as having value to an organization.
    
  - **Threats** : Any circumstance (or) event that can negatively impact assets.
    
  - **Vulnerabilities** : A weakness that can be exploited by a threat.

  - **Exploit** : It is a way of taking advantage of vulnerability.

  - **Exposure** : It is a mistake that can be exploited by a threat.


**Asset management** : The Process of tracking assets and the risks that affect them. it starts with having an assets inventory.

**Asset inventory** : A Catalog of assets that need to be protected.

## Asset Classification : 

The Practice of labeling assets based on sensitivity & importance to an organization.

Levels of asset classification

  -  Public ---> can shared by anyone
  
  -  Internal-only ---> Only to people in the organization.

  -  Confidential ---> only to specific authorized people.

  -  Restricted ---> Highly sensitive

## Data
It is information that is translated, Processed, or Stored by a computer.Protecting data is one of the most importent task for security analyst.

### States of data
  - Data in use
  
  - Data in transit
  
  - Data in rest

**Data in Use** : Data being accessed by one (or) more users.

**Data in transit** : Data traveling from one point to another.

**Data in rest** : Data not currenlty being accessed.

## Information security (infosec) :

The Practice of keeping data in all states away from unauthorized users. weak infosec is a serious problem and it can lead to things like identity theft, financial loss, and reputational damage.

## Cloud security challenges :
All service provides do their best to deliver secure products to their customers. but since data is stored in the cloud & accessed over the internet, Several challenges arise.

  - **Misconfiguration** : It is one of the biggest concerns. customers of cloud based services are responsible for configuring their own security environment.
  
  - **Cloud-native breaches** : They are more likely to occur due to misconfigured services.

  - **Monitoring access might be difficult** : It depending on the client & level of service.

  - **Meeting regulatory standards** : Practiculary in industries that are required by law to follow specific requirements such as HIPAA, PCI DSS, and GDPR.

Types of risk categories
    
  - Damage
  - Disclosure
  - Loss of information
    
## Elements of a security plan

- **Policy** : It is a set of rules that reduces risk and protects information. They are the foundation of every security plan. they give everyone in and out of an organization guidance by addressing questions like, what are we protecting and why. Policies focuses on the strategic side of things by identifying the scope, objectives, and limitations of a security plan.

- **Standards** : They concern how well we're protecting assets. in security, standards are refereces that inform how to set policies they create a point pf reference.

- **Procedures** : It is a step by step instructions to perform a specific security task.

**Compliance**: It is the process of adhering to internal standards and external regulations. At a higher level, maintaining trust, reputation, safty, and the integrity of our data are just a few reasons to be concerned about compliance.

**Regulations** : It rules set by a government (or) other authority to control the way something is done.

## NIST CSF Components

It mostly contain

  - Core
    
  - Tiers
  
  - Profiles

**Core** : it is basically a simplified version of the funtions (or) duties, of a security plan. The CSF Core identifies five broad funtions.

  - Identify
   
  - Protect
  
  - Detect
  
  - Respond
  
  - Recover

**Tiers** : These provide security teams with a way to measure performance across each of the five funtions of the core. 
it range from Level-1 to Level-4
  - Level-1 (or) passive, indicates a function is reaching bare minimum standards.
    
  - Level-4 (or) adaptive , is an indicates a function is being performed at an exemplary standard.

**Profiles** : These Provide insight into the current state of a security plan.

### Security controls

Safeguards designed to reduce specific security risks. Type of security controls.

  - Technical
  
  - Operational
   
  - Managerial

### Informational Privacy : 

The Protection of unauthorized access and distribution of data . it is about right to choose. people and organizations a like deserve the right to decide when, how, and to what extent private info is shared.

### Principle of least privilege:

The concept of granting only the minimal access and authorization required to complete a task (or) function.

### Data Owner:

The Person that decides who can access, edit, use, (or) destroy their information.

### Data Custodion:

Anyone (or) anything thats responsible for the safe handling, transport, and storage of information.

### Data Steward:

The Person (Or) group that maintains and implements data governance Policies set by an organization.

### Data Lifecycle :

It is an important model that security teams consider when protecting info. in general, the data lifecycle hass five stages.

    Collect--> Store--> Use--> Archive--> Destroy

Business Store. move, and transform data using a wide range of IT system.

## Information security (VS) Information Privacy:

Security & Privacy are two tearms that often get used interchangeably outside of this field.

**Information Security** : It refers to the protection of unauthorized access and distribution of data.

**Information Privacy** : It refers to the practice of keeping data in all states away from unauthorized users.

The key difference in privacy is about providing people with control over their personal info. but security is about protecting people choices & keeping their info safe from threats.

## Vulnerability management :

It is the process of finding and patching vulnerabilities. it helps keep assets safe, it is a method of stoping threats before they can become a problem.

It is of four step process.

  - Identify vulnerabilities
  - Consider potential exploits
  - Prepare defense against threats
  - evaluate those defenses
 
### Common CI/CD pipeline vulnerabilities:
Some of the common vulnerabilities to be aware of

  1) Insecure dependencies : Risks from third - party code.

     Action --> Regularly scan & update dependencies
     
  2) Misconfigured permissions : Controlling Access

     Action --> Implement strong access management using (RBAC)

  3) Lack of automated security testing: Missing critical checks

     Action --> Integrate automated security testing (SAST and DAST) into the CI/CD Pipeline.
     
  4) Exposed secrets : Protecting Sensitive info

     Action --> Never hardcode secrets

  5) Unsecured Build environment: Protecting the pipeline infra

     Action --> Harden your build environments.

### Building a secure CI/CD Pipeline:
To Proactively address these vulnerabilities, a layered security approach is key.

  - **Integrate security from the start** : Embrace DevSecOps
  - **Implement strong Access Controls** : Strick policies on the least privilege
  - **Automate Security Testing Everywhere** : Automated security scans & Test them as part of build & Deploy.
  - **Keep dependencies updated** : Maintain inventory of third party apps & dependencies. regularly update to patch security vulnerabilities.
  - **Secure secrets management** : Never hard code sensitive data. 

## Defense in depth:
It is a layered approach to vulnerability management that reduces risk. it is also refers to as a castle approach as it resembles the layered defenses of a castle. it can be used to protect any asset, it used in cybersecurity to protect info using a five layer design.

  1) **Perimeter Layer** : This is a user authentication layer that filters external access. its funtion only allow access to trusted parterns.
     
  2) **Network Layer** : It closly aligned with authorization. it is made up of tech like network firewall & other.

  3) **Endpoint Layer** : It refers to the devices that have access on a network. They could be devices like laptop, desktop, (or) a server.

  4) **Application Layer** : Includes the interfaces that are used to interact with technology. Security here means programmed as part of app.

  5) **Data Layer** : We have arrived at the critical data that must be protected, like personally identifiable information.

