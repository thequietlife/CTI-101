## Basics

### How Computers Work
### Computer Software

#### Applications
* e.g. Mozilla Firefox - consists of 20 million machine code instructions

#### Intro to Code
+ve of computers - can process a lot of information quickly, accurately <br>
-ve of computers - only does what is asked, it is not a human brain with a will of its own

#### How Computers Work
* code is step by step instructions for a computer to follow

#### Computers
* stupid but useful
  
#### Developers
* link the code and computer together
* when creating a new feature a developer uses their knowledge of computers, creativity and insights about user needs
* developers work out each step and write it in code for the computer
  
#### First Code Operation
* Javascript
* print("hello, world")

#### Bugs
* syntax and logic errors

#### ASCII Art
print (" *   * ")

#### Programming Languages
* rules for the code
* high level through to low level

#### Types of Programming Languages
* Compiled
* Interpreted

#### Programming Languages: Source Code
* editable
* licence to **use** the software, not change it

#### Open Source in Theory
* free to use
* Richard Stallman, Free Software Movement
* Linux

#### Open Source in Practice
* right to modify
* all developers can contribute

#### The Operating System
* e.g. Apple Mac macOS Sequoia 15.0.1 and Microsoft Windows 11
* boot-up process starts when a computer is switched on
* manages the starting, running, stopping of programs
* ensures all resources are released when a program ends
* sandboxing of programs
* allows software updates

#### Lifecycle of a Program
* loads the program
* each program gets its own **memory**

#### Ending Programs
* user closes program
* program glitches "not responding"
* running out of memory
* program tries to access the memory of another program (corrupted data)

#### OS: Reboot
* why does this work?
*   fixes a bug in the OS or hardware error
*   rebooting wipes all the memory
*   in theory not needed but in reality it seems to work a lot

#### Architecture: Machine Code
* architecture is like a guide, it helps the computer understand what to do
* each line of machine code is like one step in a recipe
* Javascript gets converted into machine code
* machine code is written in **binary**
  
_______________

### Computer Hardware

* Physical parts of a computer

#### Central Processing Unit (CPU) 
* microprocessor
* the belle of the ball
* in every computer
* not just one chip, it has three main components
  - control unit: assigns tasks
  - logic unit: in charge of math tasks
  - memory unit: responsible for memory usage
* fetches, decodes and executes

#### Chips and Transistors
* Big business selling CPUs
* Intel, AMD, Apple, NVIDIA make CPUs
* CPUs are made of a multitude of transistors
* Apple's M2 has 20 billion transistors
* transistors are like a digital switch
* solid state = no moving parts
* Moore's Law (Gordon Moore, Intel cofounder) = number of transistors on a chip doubles every few years. Compare M1 to M2

#### Memory
* a storage area for bytes
* two types
  - Random Access Memory (RAM)
  - Persistent Storage
 
#### RAM
* not persistent, if you are working in github and the power glitches, you only have up to where you last committed changes
* when you hover over a browser tab you can see the memory usage (198MB)

#### Persistent Storage
* saved even when not switched on
* e.g.  hard drive, flash drive, Solid State Disk (SSD)

#### Circuits
* helps make a toy train move
* made up of digital logic gates
    - AND gate
    - OR gate
    - XOR gate
    - NOT gate
      
AND gate: 💡 💡 both switches need to be on for the light to shine <br>
OR gate: 💡 the light shines if at least one switch is on <br>
XOR gate: 💡 the light shines if one switch is on but not both <br> 
NOT gate: topsy turvy time. if the switch is off, the light shines 💡<br>

#### The Operating System: All the Elements Pulled Together

<img
src="https://github.com/thequietlife/CTI-101/blob/95e02d6e10d1b9e672bac02df03cec65df6262b8/images/os.jpeg"
alt="three parts of the operating system. 1. CPU 2. RAM 3. Storage" width="400"/>

#### 🪛 Teardown Time

#### The Motherboard 
Sure does get dusty in there. This is an old PC I inherited. Ripe for a teardown. <br>A huge heatsink! especially compared to the teeny Raspberry Pi ones
1. CPU
2. RAM
3. Heatsink
4. I/O Controller Hub

<img
src="https://github.com/thequietlife/CTI-101/blob/93452f9f764f518278cb1c236ced034da5afce51/images/pc-1.jpeg"
alt="motherboard and all the various components" width="400"/>

#### CPU Socket
The CPU removed from its secure spot
* clip that needs to be unhooked
* little wires that connect to the CPU


<img
src="https://github.com/thequietlife/CTI-101/blob/d4e01a7fd1ccbe87c7c8caaef351c5607c41692c/images/pc-2.jpeg"
alt="CPU released out of motherboard" width="400"/>

#### CPU
The CPU flipped over
* gold spots that connect to the wires in the socket
* if we sliced it open we would see a silicon chip and resistors poking out

<img
src="https://github.com/thequietlife/CTI-101/blob/d4e01a7fd1ccbe87c7c8caaef351c5607c41692c/images/pc-3.jpeg"
alt="bottom of the CPU" width="400"/>

#### RAM
* the RAM consists of chips stuck on a printed circuit board (PCB) called a DIMM (Dual In-Line Memory Module)
* a few years earlier the chips would have been bigger. Moore's Law backed up.

<img
src="https://github.com/thequietlife/CTI-101/blob/25734a483b4288cdd2a4f467be304c95e170bd1d/images/pc-4.jpeg"
alt="RAM DIMM removed from the motherboard" width="400"/>

#### Hard Drive
* hard drive connects to the motherboard via a SATA (Serial AT Attachment) cable
* 500GB hard drive. an example of persistent storage
* it has a 3.5 inch spinning disk inside

#### BIOS
* when a computer is switched on, the BIOS checks all the parts are ready. then it tells the CPU it can get to work
__________________

### Data and Storage

### Bits and Bytes

#### Decimal Number System
* **decimal number system** is the number system we are used to: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
* all the the numbers we use daily consist of these 10 different digits
* e.g. 57, 3920, 453, 23450
* referred to as **Base 10**

#### Binary Number System
* the computer uses a Binary Number System
* only uses two digits: **0 and 1**
* e.g. 1, 10, 11, 100, 101, 110, 111, 1000, 1001, 1010

#### Bits
* solid state drive (SSD) uses electronic switches 
* these electronic switches like light switches can be either on or off
* switch on 💡 = 1 binary digit
* switch off = 0
* binary digit = bit
* so bit: 0 or 1 (off/on)
* single bits aren't very useful

#### Bytes and Words
* instead add the bits into groups
* 8 Bits = 1 Byte
* e.g. 0 1 0 1 1 0 1 0
* one byte can store one character, e.g. 'A' or 'x' or '$'

#### Bytes and Characters: ASCII Code
* ASCII: each character has a corresponding number
* e.g. 'i' = 105, 01101001
* ASCII covers only 128 characters 
* unicode expands to include math symbols, Greek amd emoji

#### Typing Texts, Bytes
* When you send a text each letter is converted to a number
* character encoding (ASCII)
* e.g. "Hi" = 72, 105
  - H = 72
  - i = 105

#### Sizes of Information Packages
* Kilobyte (KB): roughly 1000 bytes
  - e.g. an email without images is about 2KB
  
* Megabyte (MB): roughly 1000 KB; 1 million bytes
  - e.g. an email with attachments can be about 2MB
  - used to measure image sizes
    
* Gigabyte (GB): approx a billion bytes
  - e.g. early iphone's capacity was 8GB 
  - an iphone 16 pro capacity ranges from 128GB - 1TB 😱
    
* Terabyte (TB): roughly 1000 gigabytes (about 1 trillion bytes)
  - e.g. Western Digital portable hard drive (HDD) capacities range from 1TB - 6TB
 
#### Digital Media
#### Digital Compression Lossless
* **Compression** rearranges data to use fewer bytes 
* **Lossless** compresses and keeps the orginal quality
* PNG (Portable Network Graphic) is lossless, it won't loose any of its data
* e.g. PNG used for logos, hero images

#### Digital Compression Lossy
* **Lossy** compression 
* compresses but you loose some quality
* JPEG (Joint Photographic Experts Group) looses data when compressed but the advantage is that it doesn't take much space
* e.g. JPEG files are used on websites, like a blog post


#### Wrap Up
Computers need an **input** like entering your password on the keyboard to log in
**Storage** and **processing**: A computer takes the input and processes it (algorhythm)
**Output** If the password is correct you get logged in

Power On > Boot-Up > Operating System Loads > Input > Processing > Temporary Storage > Permanent Storage > Output > Networking > Cooling > Sleep







































	







__________________
Sources: 
1. [Stanford CS 101](https://web.stanford.edu/class/cs101/)
2. [How Computers Work, Ron White, Tim Downs](https://www.amazon.com/How-Computers-Work-Ron-White/dp/0789736136)
3. [Stanford CS105](https://www.youtube.com/playlist?list=PLoROMvodv4rPzLcXBhbCFt8ahPrQGFSmN)





































