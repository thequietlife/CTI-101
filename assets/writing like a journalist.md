## 🖍️ Threat Intel for Everyone: Writing Like A Journalist To Produce Clear, Concise Reports - Selena Larson

**Notes from Selena Larson's SANS CTI Summit 2021 Presentation**
_______

## Summary
* Have a TL;DR (too long; didn't read)
* ELI5 (Explain Like I'm Five)
* Conclusion of the report: Don't have new info or have the conclusion as the only place the info is simplified/broken down, easy to read  

## Summary <sup>AI</sup> 
CTI reports should be clear, concise, and audience-focused. Use a TL;DR, write at an eighth-grade reading level, and structure reports using the inverted pyramid: start with key facts (Who, What, Why), add supporting details, and include optional technical depth. Use active voice, engaging headlines, and concise leads. Summarize the report’s purpose early (Nutgraf) and ensure timely delivery. Edit ruthlessly for clarity, keeping the audience in mind. Leverage resources like *The Elements of Style* to improve writing.

### Key elements of writing CTI reports

* A crucial part of CTI is explaining things to a broad audience. Taking important subjects and packaging them in an effective and easy to understand way
* Subreddit r/Explain Like I'm Five (ELI5) - a concept that can help people better communicate their expertise to a wide audience
* Write for an eighth-grade reading level
* CTI is for everyone, make it easier for customers to read, spread and act on. Example:
  - A threat actor is using LinkedIn (LI) for open source intelligence information gathering as well as spear phishing. Finding employees working on specific projects or finding the different software services that are used at an organisation. Based on job postings or people's profiles on LI. That threat intel can be operationalised across an organisation, delivered to the HR department. So HR teams can decide what type of information they should be sharing on LI, coming up with new policies or restrictions for information sharing for employees and thinking about how they can better protect themselves from this particular threat

### Concepts journalists learn (focused on news writing)

Parallels between threat intelligence writing and journalism. 

**Inverted Pyramid of News**

* A structure for framing news writing
* How to effectively communicate and get that information across

<img
src="https://github.com/thequietlife/CTI-101/blob/b2bf9014e355294ee1bbad9f97a85c173a3ce9a7/images/inverted%20pyramid%20of%20news.png"
alt="upside down triangle - top bit: Who, What, Where, When, Why, How; middle section of triangle: Supporting information and additional facts. Tip of triangle (bottom): Detailed, in-depth info" width="300"/>

**Who, What, Where, When, Why, How**
* The most important info, shared succinctly. Bottom Line Up Front (BLUF)
* Readers should quickly understand what the report is about and why it matters
* In CTI:
  - Adversary
  - Malware
  - Victim
  - Timing
  - **Why it matters to your customers/stakeholders/audience** e.g. highlighting potential impact to xyz

**Supporting information and additional facts**
* Additional details that support the essential elements of information
* In CTI:
  - Tactics, techniques, and procedures: the how, where and the why getting fleshed out a little bit more
  - Information for defenders: actions that can be taken to prevent an attack, to recover from an attack, information for proactive defence

**Detailed, in-depth info**
* Can be deleted without changing the meaning or point of a story
* In CTI:
  - Depending on the audience, this can include technical malware analysis, attribution, related activity
  - Background information not for operational use


**Headlines aslo referred to by journalists as Head (Hed)**
* You want to provide as much information in as few words as possible
* You want the reader to learn something and want to continue to read the report
* Report titles = Headline
* Use of "How" indicates the reader will learn something
* Example:
  - [How U.S. agencies’ trust in untested software opened the door to hackers](https://www.politico.com/news/2020/12/19/how-federal-hack-happened-448602)
  - [Threat actor leverages coin miner techniques to stay under the radar – here’s how to spot them](https://www.microsoft.com/en-us/security/blog/2020/11/30/threat-actor-leverages-coin-miner-techniques-to-stay-under-the-radar-heres-how-to-spot-them/)
 

**Lead (Lede)**
* Brief one or two sentence statement that opens the report
* Includes important aspects of the story
* Draws reader in

With the Politico news story we are learning that the reason why the adversary was able to access the U.S. government and exploit the supply chain is because "no one was looking in the right place". This provokes the reader to think about where is the right place, how did they do it? It encourages the reader to continue reading.
<img
src="https://github.com/thequietlife/CTI-101/blob/1738db3d4ccf03ef886c6ea6e8b140ad4205e495/images/how-federal-hack-happened.png"
alt="cyber news story lead: no one was looking in the right place" width="300"/>

The Microsoft report's lead explains what cryptocurrency miners are, what is this threat and how does it take advantage of low-priority alerts.

<img
src="https://github.com/thequietlife/CTI-101/blob/1738db3d4ccf03ef886c6ea6e8b140ad4205e495/images/threat-actor-leverages-coin-miner-techniques-to-stay-under-the-radar-heres-how-to-spot-them.png"
alt="CTI report lead: cryptocurrency miners are typically associated with cybercriminal operations, not sophisticated nation state actor activity...BISMUTH take advantage of the low-priority alerts" width="300"/>

**Nutgraf (short for nutshell paragraph)**
* The entire point of the story or report **in one paragraph**
* Describes what is new, important and why readers should care
* Nutgraf is like the Executive Summary
* The important info needs to be up high not sprinkled throughout or in the conclusion
  
Both examples are "crunchy, with lots of nutritious information" 
The Politico article spells out how the blind spot was created, how hackers took advantage of it and what a supply chain attack is.
<img
src="https://github.com/thequietlife/CTI-101/blob/6cc36816e74e1c27bc64a1117da5fa5132c576da/images/politico%20nutgraf%20example.png"
alt="cyber news story nutgraf:that created the blind spot...embedding code in widely used network management software" width="300"/>

The Microsoft report talks about how BISMUTH uses open source tooling historically and the important part is that over the summer the group started to deploy this Monero coin miners.
<img
src="https://github.com/thequietlife/CTI-101/blob/6cc36816e74e1c27bc64a1117da5fa5132c576da/images/Microsoft%20nutgraf%20example.png"
alt="CTI report nutgraf: custom and open-source tooling to target large multinational corporations, governments, financial services, educational institutions, and human and civil rights organizations...deployed Monero coin miners" width="300"/>

**Conclusion**
* News writing often has "kickers", something that is going to be very memorable. Sometimes it's funny, compelling or interesting
* Threat intelligence reporting should have conclusions
* Restate important information, calls to action and why it matters to customers
* You want the reader to leave feeling a particular way and potentially take certain actions. It is the "So What?" of your entire report. Make it super memorable to a reader
* **Make sure the conclusion is not the only place where information is simplified and summarised**

**How to be a much better writer**
Edit your report. Don't have a personal attachment to your words and writing. Need to be able to take the red pen to it and really cut it down or your editor will. "Murder your Darlings", Sir Arthur Quiller-Couch

**Deadlines**
* Journalists: You want to be accurate and get information out there first
* [CART: The 4 Qualities of Good Threat Intelligence](https://www.activeresponse.org/the-4-qualities-of-good-threat-intelligence/)
  - Completeness
  - Accuracy
  - Relevance
  - Timeliness
* Timeliness: Being able to produce efficient writing that meets deadlines is key
* Implementing deadlines for intelligence reporting is extremely valuable. It helps you:
  - know when you need to inform customers
  - adhere to a threat intelligence reporting cycle

**Threat intelligence writing**
* Still keep hunting and finding new, important information
  - Collect
  - Analyse
  - Publish: once you get enough to information that can support the intelligence requirements of your audience. You want to make sure you are getting the material out there and publishing it
  - **We are not just writing for other analysts**
  - We are writing for our stakeholders, decision makers, people dealing with patch management, business decisions, security operators. Who are also experts in this field. Think about the **audience** and how you are writing, presenting and publishing information.
 
**Passive Voice**
* Passive voice removes urgency, makes to difficult to process and think about how to take action on something
* Avoid "helping verbs":
    - am
    - is
    - was
    - were
    - able
    - been
 
* Example:
    - **Don't do this**: The company *was targeted by* APT29 (passive)
    - **Do this**: APT29 *targeted* the company (active)
* No big words. Readers should not need to look at a dictionary or thesaurus while reading
* At times an uncommon word needs to be used. The word needs to be defined in the sentence
  
**Clean Up Your Writing**
1. Be concise
2. Keep sentences short and simple
3. Put the most important information first
4. Consider your audience
5. Remove passive voice

**Resources**
* The Elements of Style, William Strunk
* Poynter.org [These tips will make you a better writer](https://www.poynter.org/reporting-editing/2019/these-tips-will-make-you-a-better-writer/)
* [Purdue University Online Writing Lab](https://owl.purdue.edu/owl/)

__________________
Sources:
1. [Threat Intel for Everyone: Writing Like A Journalist To Produce Clear, Concise Reports - Selena Larson, SANS 2021 CTI Summit](https://youtu.be/gqsE2coucjg?si=IHRhqxU1eDHtTdTB)



    
