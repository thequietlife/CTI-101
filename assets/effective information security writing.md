## 📝 Effective Information Security Writing - Chris Sanders

Notes from Chris Sanders Applied Network Defense Course

## Summary
* xx
* xx


### Why writing scares us

* **Fear of not sounding competent** – Overthinking leads to slow, overly complex writing.
* **Worry about missing key points** – Anxiety over leaving something important out.
* **Self-doubt about writing ability** – Feeling like a "bad writer."
* **Fear of being wrong** – Concern about making mistakes or being incorrect.
* **Imposter syndrome** – Feeling unqualified to write or share ideas.
  
### Overcoming a fear of writing
* The Prism Strategy
  - **Your perspective is unique** – Even familiar topics gain new life through your lens.
  - **Personal experience adds value** – How you learned something matters as much as what you learned.
  - **Originality comes from viewpoint** – It’s not about being first, it’s about being *you*.
  - **Your voice can be the one that makes it click** – Even if others have covered the topic before.
  - **Unique framing matters** – Your approach may resonate where others didn’t.
  - **Personal insight creates connection** – Sharing how *you* understand something helps others understand it too.
  - **Impact isn't about being first** – It's about being relatable, clear, and human.
* Set up an Advisory Board
  - find people who can review you writing but also people who you are okay with getting feedback from.
* Keep a journal
  - Capture the crazy thoughts bouncing around.
* Write more publicly

### Why is communication important?
* Wide range of writing we do:
  - status reports
  - case notes
  - meeting notes
  - slack chat
  - email etc
* We spend 20-30% of our day on communication related tasks
* So we need to do it well, e.g. "I get frustrated that the organisations I assess don't ever implement my recommendations, even a year or more after I compromise their network" - this can be remedied by **becoming more convincing** in your writing.

### On writing
* Your writing lasts a long time, e.g your investigation notes may be referred to down the track by others
* Once you write something, the words belong to your reader and their meaning can change
* How you express your findings and your technical work will dictate a portion of your future success
* An analyst needs to be good at reading the things people want to read about.

### Course outline
1. Telling a story - Chris' big secret to writing good content
2. Common writing mistakes - word choice and structure
3. Writing penetration testing reports
4. Forensic writing - incident response (compromise) reports, malware analysis reports and case notes
5. Tips


### Telling a story
* Technical writing can use some aspects of creative writing
  - Imaginative
  - Entertain
  - Captivate
  - Evocative
* The content can be factual whilst also being **imaginative**. E.g. You can describe the actions malware took and then pivot to a discussion of how you could have caught it sooner if you had better endpoint visibility. Or the destruction that could have been wrought if the malware decided to override the master boot record of the infected server.
* Creative writing makes things much more readable. Add a richer description of what happened.

<br>

**Your writing has to tell a story**

* People remember things they emotionally connect with
* They emotionally connect with things that they can relate to
* Put the reader in your shoes and make them experience it as you did
* **Build empathy**

<br>

1. Tell a real story
2. Adapt previous stories
3. Make one up to illustrate your point

* Referred to as a 'what if analysis', where you branch a real story into a series of hypothetical scenarios to plan for potential future scenarios. Combine technical and creative writing to hook your reader.
* Use the stories to persaude your reader into taking an action, e.g. better securing your network or devoting more resources towards security monitoring.


### Elements of a story

Character ➡️ Setting ➡️ Conflict ➡️ Theme ➡️ Plot 

* An investigation can translate to a story

#### Developing plot

* Characters, theme, conflict and setting ➡️ plot
* For an investigation we know what happened. We know the events that took place. This is the plot
* The plot is our storyboard and how we express the truth of our knowledge
    - Pen Test: first hand knowledge of movement through the network and putting it into narrative form
    - Incident Response (Compromise) Report: timeline of attack drawn from evidence. Writing down the actions of the attacker - the story is pretty much there
    - Malware: timeline of malware execution drawn from analysis

##### Story arc
* Intro ⬆️ Rising Action/Conflict ➡️ ➡️ Climax 🌈 ⬇️ Falling Action ➡️ Resolution
* 🌈 Your writing needs to have an arc
* Introduce characters in the rising action
* Recommendations and call to action should be in the resolution but allude to them in other parts of your writing
* Going through the complete sequence of your plot doesn't mean you have to write a 50 page doc. You can construct an **entire plot in a paragraph or two**. E.g. a pen test finding - the finding will represent a complete story arc in a paragraph or two. This applies to **emails** and **case notes** too
* Stories within stories - your report might be a broader story and the **recommendations might be smaller stories within the broader story**

##### Characters and settings
* Characters and settings - we already have this
* Characters may change
* Setting usually remains the same e.g. our network or the victim network we are targetting
* Character features: <br>
      - Qualities, Traits e.g. stubborn, loyal, chatty. Steve is a little negative but a really friendly chap. This piece of **ransomware**, it's **loud** and **boisterous** and a bit of a jerk. We can describe files and computers with human personality traits. Ransomware infects your computer, encrypts your files, makes you pay to decrypt them or else it deletes them, sounds like a jerk move. <br>
      - Motives, Purpose, Goals. What drives characters altruistic good, destructive evil, money and/or power? The ransomware and malware is motivated money and/or power. A web server is motivated by availability and speed. Your reader will get a sense of motivation, traits, qualities and purpose based on the actions of the character. By showing the reader rather than by telling them they will relate and care.
E.g. We can see Darth Vader is bad by the things he does. Luke Skywalker shows virtuous characteristics by his actions. We weren't told Luke was a good guy we could draw that conclusion ourselves.
  
* Where the work is: <br>
      - 🆓 Free: The plot, setting and characters are provided by the event that has taken place
      - 💰 Expensive: **Theme**, **conflict** are the things we need to identify and bring them out in your story. These are where a lot of technical writing fails. Here we want to control the reader and what they think. All writing is to some degree persuasive. <br>
          - **Theme**: What do you want? Something bad happened and it could happen again if my recommended course of action is not accepted. <br>
            🟦 Outcome - your recommendation is that adblockers are installed on all workstations <br>
            🟦 Investment <br>
            🟦 Trust <br>
          - **Conflict**: Why do you need it? <br>
            🟪 Good vs. evil - your story describes the conflict between good and evil. e.g. your pc user and the malicious ad they clicked on <br>
            🟪 You vs. visibility <br>










































__________________
Sources:
1. [Chris Sanders Effective Information Security Writing, Applied Network Defense](https://www.networkdefense.io/library/)
