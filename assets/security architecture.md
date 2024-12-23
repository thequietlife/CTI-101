## 📐 Security Architecture

### Summary
**Essential Security Principles**
*  Defence in Depth
*  Least Privilege
*  Separation of Duties
*  Secure by Design
*  K.I.S.S  

**CIA Triad**
* A checklist for IT projects

**Frameworks**
*  NIST Cybersecurity Framework (CSF)
  * A comprehensive checklist to ensure you have covered everything  
_______________

### What is Security Architecture?
It is the strategic design of systems to protect, information and ensure its integrity, confidentiality and availability against threats.

### Main Objectives of Security Architecture
To reduce the risk of security breaches and protect organisations from threats. The aim is to avoid a single point of control. For example, one person can not approve an invoice and process it for payment.

### Five Security Principles to Follow (and One to Avoid)
#### 1. Defence in Depth <br>
Aims to provide a number of layers to thwart a threat actor. Like American Ninja Warrior.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/08/American_Ninja_Warrior_Fly_Wheels_obstacle_Indianapolis_2016.jpg/440px-American_Ninja_Warrior_Fly_Wheels_obstacle_Indianapolis_2016.jpg"
alt="American Ninja Warrior course close up of Fly Wheel" width="200"/>

Don't rely on one single security mechanism to keep the network safe. 
🏰 Think of a castle, a building with thick, high walls. Built robustly to keep the kingdom safe. 

<img src="https://github.com/thequietlife/CTI-101/blob/442c9b622e7fa00575bbc38894c11c1a953cc2d0/images/castle%20no%20door.png"
alt="castle with no door" width="200"/>

But it needed a door. And the door added a weakness to the castle. Security was added with a bolt and gate. But that didn't provide enough protection.

<img src="https://github.com/thequietlife/CTI-101/blob/442c9b622e7fa00575bbc38894c11c1a953cc2d0/images/castle%20door.png"
alt="castle with a door" width="200"/>

So a moat was added to give an extra layer of security. 🐊 And crocodiles.

<img src="https://github.com/thequietlife/CTI-101/blob/442c9b622e7fa00575bbc38894c11c1a953cc2d0/images/castle%20moat.png"
alt="castle with a moat - ring of water surrounding the castle" width="200"/>

A system of security mechanisms.

<img src="https://github.com/thequietlife/CTI-101/blob/d8e2223f2c27f73e33fc0c44c173947b7d29d9b3/images/modern%20security.png"
alt="image shows layers involved in a user browsing the web on a network and the security measures that can be put in place" width="800"/>

<img src="https://github.com/thequietlife/CTI-101/blob/788b175aa5b848df6d6b5b9b6ed89585b3d20cc0/images/def%20in%20depth%20tools.png"
alt="following on from the previous image. shows what mechanisms can be put in place" width="800"/>

🛡️ Modern security takes a layered approach like the olde worlde castle example. We are not relying on one tool to do all the protecting. Each part of a network can have tools added to it. For example, MFA, MDM, EDR, firewalls, vulnerability testing, 🔒 encryption. <br>

#### 2. Least Privilege <br>
Giving people access to only what they need to do their job and only for as long as they need that access. 📅
<br> For example giving an employee access to only the floor they work on rather than access to all floors of the building.

<img src="https://github.com/thequietlife/CTI-101/blob/8a5b9c98f2667bcc1cf97a1c022bd789710888f5/images/least%20priv%201.png"
alt="image shows a web server with HTTP, FTP and SSH services connected" width="200"/>

<img src="https://github.com/thequietlife/CTI-101/blob/577d34bbf0de822faf4748affdd9effdf4fca853/images/least%20priv%202.png"
alt="image shows the web server with FTP and SSH services removed" width="200"/> 

Remove access to services that are not needed like remote access into a server. Change 'Admin' to another name, change all the default passwords. These are ways to reduce our attack surface and vulnerability. 

**Privilege Creep** When an employee moves to a new project or role and keeps all the same access, gets more access and maybe also is given 'just in case' access. This can be mitigated by regular reviews of access rights.

#### 3. Separation of Duties <br>
🪜 Ensures no single person has complete control over all aspects of a critical process or task. A manager has authority approve a timesheet or invoice which then goes to the finance person for processing. Another example is a developer asking IT for access to a database.

<img src="https://github.com/thequietlife/CTI-101/blob/63fb2904ec9990bbec90414bf0a3ea82c77b81bb/images/duties.png"
alt="image show a person at a desk with an arrow going to another person at a desk with a tick and cross above them. An arrow then goes to an action like a database" width="300"/> 

#### 4. Secure by Design <br>
Incorporating security from the start and at each stage of a project, all the way from design to deployment and the maintain phase (continuous improvement). 

<img src="https://github.com/thequietlife/CTI-101/blob/567e780bced7dddf2e6a6774dc8f69a5395e1b8c/images/SDLC.png"
alt="stages of the software development lifecycle. the deploy stage is highlighted" width="300"/>

It is too late to consider security at the deploy stage.

<img src="https://github.com/thequietlife/CTI-101/blob/44ab3a1f99126647d2d18a8c66c7b6333095a09f/images/SDLC%20sec.png"
alt="stages of the software development lifecycle repeated but with security in the centre and pointing to each stage" width="300"/>

Security needs to be incorporated at each stage. Look at the requirements through a security lens &rarr; build security into the design &rarr; secure code principles &rarr; install on a secure system &rarr; testing and guarding the test data &rarr; consider security in CI.

🔐 📦 Secure out of the box.

#### 5. K.I.S.S. <br>
Make the system secure but also as simple as possible. If it is too hard to do the right thing, users go with the easier way which will usually be the wrong thing. E.g. using one password for multiple applications. The system needs to be complex enough to keep threat actors out. But not so complex for our users to do the right thing.

#### X. Don't do this: Security by Obscurity <br>
Relys on secret knowledge to keep a system secure. E.g. A house with a secret room. The room is opened by knowing which book on the bookshelf opens the door. 

<img src="https://github.com/thequietlife/CTI-101/blob/baa2e05b6fafcd6662e02f1619c1871e7fbae4ef/images/black%20box.png"
alt="shows black box security - the algorhythm is secret known only by the founder" width="300"/>

<img src="https://github.com/thequietlife/CTI-101/blob/baa2e05b6fafcd6662e02f1619c1871e7fbae4ef/images/glass%20box.png"
alt="similar to previous image but the box is clear and shows cogs" width="300"/>

We want glass box security not black box security. Glass box security uses industry recognised algorhythms like NIST's Advanced Encryption Standard (AES). This is an algorhythm that anyone who is interested can look into it and see how it works.
__________________

####  Confidentiality, Integrity, Availability (CIA) Triad
The CIA Triad is a framework that helps guide the protection of data and systems. 
The three principles are: 
* Confidentiality
* Integrity
* Availability

<img src="https://github.com/thequietlife/CTI-101/blob/c9ae0dd1cc179b5e5b3b7928f26abf611a7c8f35/images/CIA%20Triad.png"
alt="triangle with a text on each side - confidentiality, integrity, availability" width="300"/>

**Confidentiality**: Sensitive data is available only to authorised users. <br>
How?
* Access control: via authentication and authorisation (e.g. MFA and role based access control (RBAC))
If the user is who they claim to be and they have the privileges. The user is let into the system.

<img src="https://github.com/thequietlife/CTI-101/blob/203dadf2596f8f174814aaa10b52768459e923dd/images/MFA%20and%20RBAC.png"
alt="image shows an authorised user is who they claim to be and gains access via MFA, they also have the required privileges and gain access to the database" width="300"/> 

If an unauthorised user trys to authenticate to get into the system and they do not have the right credentials they are denied access. Or they access the system and are able to authenticate, but they do not have the privileges, they are not allowed access. 

<img src="https://github.com/thequietlife/CTI-101/blob/837ec7720d7ca4c5b54976c60a6f94c7c408e763/images/non%20auth%20user.png"
alt="image shows a person trying to access a system via MFA, even if they get through MFA they do not have the correct privileges to get in" width="300"/>

* Encryption

When I want to send a message to my buddy, an authorised user, I want to make sure that only they can read it. I can do this by using encryption. The message is encrypted with a key, a cryptographic key, which is a string of bits. My buddy has the very same key, called symmetric encryption, and is able to decrypt the message and read it.

<img src="https://github.com/thequietlife/CTI-101/blob/86ec308519d5ac43c5a6cf3a868121a763316a86/images/encryption.png"
alt="image shows a person sending a message to an authorised user, the message is encrypted so that an unauthorised person can not read the message" width="300"/>

This other person does not have the cryptographic key and can not decrypt the message.
  
**Integrity**: Only authorised users can make changes to data. If data gets modified then it can be detected. And if it is detected we know not to trust it and we can take necessary steps.

<img src="https://github.com/thequietlife/CTI-101/blob/7f255657bb797060c5c6bb4bfa9617440c2854b0/images/integrity%20good.png"
alt="image shows authorised person using a system and their actions are recorded in the syslog" width="300"/>

<img src="https://github.com/thequietlife/CTI-101/blob/fa8608b1159a06590721c1f8e459cadb8c5bb007/images/integrity%20bad.png"
alt="image shows an unauthorised using elevating their access to super user and deleting the changes they made in the system" width="300"/>

**Cryptographic Functions**
**Digital signatures** and **message authentication codes** are used to tell if there has been a change. Detection &rarr; Appropriate countermeasures.

**Availability**: Sensitive data should be visible and accessible whenever needed to authorised users. <br>
An example of basic **Denial of Service**: <br>

<img src="https://github.com/thequietlife/CTI-101/blob/3234efdab8a8e49257708414529436a23b680274/images/denial%20of%20service%20-%20basic.png"
alt="an authorised user accessing a web server to do a legit transaction and an anauthorised user sending repeated requests" width="200"/>

The unauthorised user is flooding the system with transaction requests, faster than the system can respond to them. When the system can't provide service to authorised users this is called a Denial of Service.

A more complex example of Denial of Service, a **distributed denial of service** attack: <br>

The attacker has now also taken over unsuspecting user's computers. The threat actor can send one command to get these systems to also flood the web server with traffic. This will crash the web server even faster due to this force multiplier.

<img src="https://github.com/thequietlife/CTI-101/blob/a851ae083a42aab0648480135d0128754853f988/images/DDOS%20example.png"
alt="similar to above image but more user computers have been overtaken and are flooding the system with requests" width="300"/>

This is also called a botnet.

<img src="https://github.com/thequietlife/CTI-101/blob/08e250ed9a51143ec4d58e8f543a3534ac4e67be/images/SYN%20Flood%20.png"
alt="shows attacker sending SYN packets but doesn't complete the handshake" width="300"/>

Another example of a Denial of Service, SYN flood attack
The attacker is sending SYN packets but doesn't complete the handshake. This leaves the server with half-open connections and ties up the server's resources.

We need to guard against these attacks, make sure that our systems are available to our authorised users when they need it.

#### CIA Triad in summary:

IT project checklist: <br>
✅ Have I met the confidentiality requirements of the project? Is the sensitive data only available to authorised users? <br>
✅ Is there integrity checking? If someone modifies or tampers with the system will I be made aware of it? <br>
✅ Do I have the system available all the time it is supposed to be available? <br>

#### Cybersecurity Architect
* Role
* Mindset
* Tools
* Domains

<img src="https://github.com/thequietlife/CTI-101/blob/fe4019ecf881cf3064f70b3b08a6ec41a70cc8cf/images/Roles.png"
alt="shows flow of cybersecurity architecture from whiteboard to rollout by engineers" width="400"/>

The security architect thinks about how will the system fail and what do I need to put in place to guard against that?

🔧 Cybersecurity Architect Tools
* Business context diagram
    * shows relationships between different entities in the system; high level
* System context diagram
    * shows how external entities interact with an internal system 
* Architecture overview diagram
    * drills down a further layer; shows all the elements that are part of a system

A security architect will look at each layer, they need to understand how the system works and how the system might fail.

**Frameworks**

The [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)

<img src="https://github.com/thequietlife/CTI-101/blob/33920bcf5ffeecfb285e33b1da2c280f9e655b02/images/NIST%20CSF.png"
alt="shows the functions of the NIST Cybersecurity Framework (CSF)" width="200"/>

📖 A set of guidelines: <br>
✅ Identify: the organisation's cybersecurity risks are understood; e.g. what are the critical business processes and assets? <br>
✅ Protect: Safeguards to manage the identified risks are in place; e.g. manage access, levels of encryption <br>
✅ Detect: Possible attacks and compromises are found and analysed; e.g. monitor networks, systems to find incidences <br>
✅ Respond: Steps to take when an incident occurs; e.g. ensure everyone is aware of their responsibilities with the incident response plan <br>
✅ Recover: Assets and operations are restored; e.g. execute recovery plan, communication with stakeholders <br>

In reality quite often a security architect is called in towards the end of a project. The best practice would be to bring in the security architect at the **risk analysis** stage of the lifecycle.

### **Cybersecurity Domains** that are the focus of security architects

<img src="https://github.com/thequietlife/CTI-101/blob/411252b1d8799927c906a4cd6935a58b12300efa/images/security%20domains.png"
alt="shows the seven domain that security architects focus on" width="400"/>

1. Identity and Access Management (IAM)
2. Endpoint
3. Network
4. Servers
5. Data
6. Monitor
7. Response

### **Identity and Access Management (IAM)**

Previously the network was regarded as the perimeter. Firewalls and endpoint protection do not provide enough security.
Now identity is regarded as the new perimeter.

**4 A's** <br>
✅ Administration <br>
✅ Authentication <br>
✅ Authorisation <br>
✅ Audit <br>

**Administration** - we try to figure out what access rights you have and create those
**Authentication** - we determine who you are
**Authorisation** - we assess if you are allowed to do this or not
**Audit** - review if we did the previous 3 A's correctly

Best practice would be to have one directory:

<img src="https://github.com/thequietlife/CTI-101/blob/f8070a669e6d2a5d1c13152ed87e8d25a9531216/images/one%20directory.png"
alt="shows each system like email, HR, CRM being funnelled into one big directory" width="800" />

In practice it is more likely that companies would have a directory for each system:

<img src="https://github.com/thequietlife/CTI-101/blob/f8070a669e6d2a5d1c13152ed87e8d25a9531216/images/separate%20directories.png"
alt="shows each system like email, HR, CRM having separate directories" width="700"/>

**IAM Architecture**

1️⃣ Have a place to store users <br>
2️⃣ A way to synchronise users information so that we have an ecosystem of integrated directories

The foundation of an IAM architecture: 
<img src="https://github.com/thequietlife/CTI-101/blob/a9eaea6633361a04b3e46d5d35cfb6bb91743d33/images/IAM%20base.png"
alt="shows the base of IAM architecture - one layer is store, above it is sync" width="400"/>

✅ Administration <br>
**Identity Management** This is where we create, delete accounts accounts and change privilege levels. Also referred to as **Identity Governance**.

**Provisioning process** - a system that effectively creates access rights: 
New starter > request access > access based on role > approval needed > Y/N access

**De-provisioning process** - with terminated employees we need a system that is even more efficient at removing those access rights, because that is where the security exposure exists.  

Terminated employee > HR system flags this person is no longer employed > that sends a request into our Identity Governance system - which will know all of the accounts that this user has > admin sends the de-provision request > no approval is needed it will just delete the access rights for that user.

We have a single source of truth. We know exactly what accounts the user has. Otherwise you would need to audit each system to check where the user has access rights and how to remove them all.

✅ Authentication <br>
The aim of authentication is to answer the question, "Who are you?" <br>
We determine who you are based upon:
* something you know e.g. password or a PIN (referred to as knowledge-based authentication) 
* something you have e.g. 📱 SMS or push notification on your mobile phone
* something you are e.g. biometric - facial recognition or a fingerprint scan

The best authentication systems don't rely on any single one of this factors. Multi-factor authentication (MFA) is used instead. Using something you have and something you are is two-factor authentication (2FA). <br>

The trend is moving more towards **passwordless authentication** and using multi factors is a way to mitigate the risk of not having any password at all. <br>

Another option is using **Single sign-on (SSO)**. The user logs into a SSO and proves who they are once (with MFA as well). The SSO system then provides the credentials for that user. The user is happier with this method. We have a unique situation where the security is better and the user is happier at the same time. 

✅ Authorisation <br>
The aim of authorisation is to answer the questions, "What are you supposed to do? Are you permitted to do that?" <br>
The authorisation system might use **Risk-Based Authorisation** or **Adaptive Access**. Which checks for certain criteria:
* your location e.g. access will be denied if you are from an unknown location. This is the risk assessment part of the authorisation
* request type e.g. checking your account balance is low risk but transferring funds might have more restrictions put on that process
* request amount e.g. you can transfer $1K but higher amounts will have extra controls
* frequence e.g. an alert may get triggered of you try to do 30 of these transactions in a day when you normally do it once a month

Authorisation is a complex algorithm that goes into all of this, and that's how we consider, based upon who you are, what you're permitted to do, are you permitted to do this or not?

A special case of access management called privileged access management, privileged user management or privilege identity management. These are types of users that have very highly privileged access: <br>
⏹️ root level access to a server <br>
⏹️ system administrator (sysadmin) <br>
⏹️ database administrator <br>
⏹️ network administrator <br>

🔑 🏰 They can control everything. They can steal all of the data or they can keep all the data safe. They can make the network secure, of they could leave it wide open. We are giving them a lot of trust. We need to put in extra verification to make sure they are doing their jobs as expected. 
<br> 🤐 But there is a dirty little secret of IT. In a lot of organisations these super sensitive accounts, do the exact of what we tell our end users to do, to have separate unique passwords and change them all the time. They tend to use 'root' and the same password for each of the systems, sometimes 300 - 3000 different systems. <br> 
But what happens when one of the sysadmin or network administrator leaves? Does the account name and password change? Generally not. <br>
What happens when one of the sysadmin or network administrator's makes a mistake. If they are all using the same log-on details how do you know who made the mistake? <br>

**Best Practice**
Put in a Privileged Access Management (PAM) system. A PAM system will require that these users with highly privileged access not log directly into the system, they log into the PAM system. <br>
The PAM requires these users to:
* use MFA
* have their own unique password. They checkout the system make the needed changes and then check the system back in. The PAM system changes that password every time someone checks out that particular account. <br>

Advantages of the PAM:
* it provides a record of who did what
* session recording - recording each keystroke.

This is helpful for two reasons. It provides an audit trail and also the sysadmin or network administrators are less likely to do things they shouldn't if they know their activity is being monitored.
  
✅ Audit <br>

This step is to make sure the previous three steps, **Administration**, **Authentication** and **Authorisation**        have been carried out correctly. 

<img src="https://github.com/thequietlife/CTI-101/blob/0da0d0b4cb30d01cdb4c763cf9001ec8e043de6f/images/UEBA.png"
alt="shows a regular user checking into the system making some changes and exiting. also shows someone with malicious intent creating an account, copying a database and then deleting it." width="200"/>

The first user logs into the system, makes some changes and logs backout. All of these actions are being logged so they can be reviewed later if needed. <br>
Another user logs in with the stolen the privileged account user's password. They have malicious intent. They create a new account, copy a database and then delete the account. All these actions were done within a small span of time and that could indicate a problem. <br>

So we need a system that audits activity, looks at all the log records and looks at different activities. It has policies and uses mackine learning to pick up some of these patterns. Enter **User Behaviour Analytics (UBA)** or **User Entity Behaviour Capability (UEBA)**. 

That wraps up the **4 A's**: <br>
✅ Administration <br>
✅ Authentication <br>
✅ Authorisation <br>
✅ Audit <br>

By covering the 4 A's we have a fairly complete architecture. All of the parts working together. 

<img src="https://github.com/thequietlife/CTI-101/blob/a736cc5483ecd7dfc83fc1e944db760a8efaecaa/images/enterprise%20IAM.png"
alt="Shows base IAM levels store, sync. Middle layer: admin, roles, access, PAM. And layer on top of federation." width="300"/>  

If we are wanting **Enterprise Identity and Access Management**, we might want to also add Federation Capability. If my organisation and employees need to log on to a SaaS system. We will need to extend the above into other identity domains. This is called a **Federation Capability**. It allows an employee to log in to my organisation's system as my identity provider and then be able to access other systems as service providers. This is also referred to as **Workforce Identity Management**. <br>
One other aspect to consider is **Consumer Identity and Access Management (CIAM)**. CIAM looks at some of these similiar capabilities with the ability to focus more on the areas that need more security like protecting privacy.

### **Endpoint**

**What** is Endpoint Security? It's about have a trusted platform. 

#### Hardware 
From a hardware perspective it involves different computing platforms. 

<img src="https://github.com/thequietlife/CTI-101/blob/e58349a23eb9cb8dc1d0f7a12f74a86ca9cac437/images/endpoints.png"
alt="shows a range of hardware including server, desktop computer, laptop, mobile, IOT device - Amazon echo" width="300"/>

We need to look at every device in holistic terms e.g. see the server as a computing platform, an software engineer's desktop system, laptop system, mobile device. These are the hardware platforms that are on our networks. We are using our personal devices to enter the corporate network. The distinction between personal devices and business devices does not exist anymore. 

This is all part of the scope security architects need to consider. Hence the need to use a holistic view and look at all of the endpoints that are out there. <br>

<img src="https://github.com/thequietlife/CTI-101/blob/94047351123cda60ff418f32c0170d87f3c9371d/images/attack%20surface.png"
alt="same as previous image but shows that all devices open up the attack surface" width="300"/>

Each of these devices is contributing to our **Attack Surface**. Each device has different vulnerabilities. The expanding attack surface is creating a lot of challenges from a hardware perspective. <br>

#### Software

We need to also take into account the software, different operating systems, that is on these devices.

* Windows
* macOS
* Linux
* Mainframes
* iOS
* Android
* IoT OS

Each of these brings more complexity, vulnerabilities and expands the attack surface. And this is why we need controls.

**Controls**

Security controls we need to put on endpoints.

<img src="https://github.com/thequietlife/CTI-101/blob/db20508fc8a739229c2d76151aa3b59057db9255/images/controls%20-%20typical.png"
alt="shows typical way controls are managed. one admin looks after server, one admin for laptops and desktops and another admin for mobiles. Prob nothing in place for IoT" width="300"/>

This is a common setup for organisations, multiple administrators managing different platforms. One administrator looks after servers, one administrator for laptops and desktops and another admin for mobiles. And quite possibly nothing in place for IoT devices. On the plus side the admins are domain experts in those particular areas. But this is not the most efficient or simplest approach.

**Best Practice - Endpoint Security Management System** <br>
A better approach would be to implement a single security policy across all of the different platforms with one console.

<img src="https://github.com/thequietlife/CTI-101/blob/4710a29a65a7e683ca3fc34701413988ba0a9bde/images/controls%20-%20best.png"
alt="shows best practice of having a single security policy and managing all the assets together" width="300"/>

This approach allows the admin to push down policies and patches across the entire infrastructure. Also the platforms can push up information and alerts into the one console. This reduces the complexity, increases visibility and is much more efficient.

**Types of Controls (Policies)** 

* Inventory - carry out an audit of all the different systems, find out hardware and software levels of existing devices and maybe discover some new ones
* Security Policy for the organisation - dictates what types of hardware and software is permitted on the network
* 




________
Sources: 
1. [What Is Security Architecture?, Palo Alto Networks](https://www.paloaltonetworks.com/cyberpedia/what-is-security-architecture)
2. [Cybersecurity Architecture, Jeff Crume IBM Technology](https://www.youtube.com/watch?v=jq_LZ1RFPfU)
3. [Describe the basic concepts of cybersecurity, Microsoft](https://learn.microsoft.com/en-us/training/paths/describe-basic-concepts-of-cybersecurity/)



