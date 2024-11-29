## 📐 Security Architecture

### What is Security Architecture?
It is the strategic design of systems to protect, information and ensure its integrity, confidentiality and availability against threats

### Main Objectives of Security Architecture?
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
* Access control: via authentication and authorisation (e.g. MFA and role based access control/privileges)
* Encryption
  
Integrity: Only authorised users can make changes to data.
Availability: Sensitive data should be visible and accessible whenever needed.





__________________
Sources: 
1. [What Is Security Architecture?, Palo Alto Networks](https://www.paloaltonetworks.com/cyberpedia/what-is-security-architecture)
2. [Cybersecurity Architecture, Jeff Crume IBM Technology](https://www.youtube.com/watch?v=jq_LZ1RFPfU)
3. [Describe the basic concepts of cybersecurity, Microsoft](https://learn.microsoft.com/en-us/training/paths/describe-basic-concepts-of-cybersecurity/)



