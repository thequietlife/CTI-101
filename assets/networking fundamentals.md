## Networking Fundamentals

### Summary
When I type in google.com in a web browser and hit enter what happens? The way that the information goes from my web browser and gets communicated to the server at google. The OSI model is how it happens (DNS Lookup → TCP Connection (Three Way Handshake) → HTTP Request → Server Response → Rendering of the Web browser page → Displaying the page).

### What is the Internet? 

The internet is a network of networks. It links billions of devices together all around the globe.

### How does the Internet Work?

If you are in a cafe using wifi, the bits get sent through a wireless router and then are transformed to the physical wire to travel the really long distances of the internet. The physical method for sending bits may change in the future. e.g. lasers sent between satellites or radio waves from balloons or drones. But the binary representation of information and protocols for sending that information and receiving that information have pretty much stayed the same.

### Bit Sending

Everything on the internet - emails, cat videos - all come down to these ones and zeros being delivered by electronic pulses, light beams, radio waves.

### IP Addresses + DNS

Networks need to be able to talk to one another. Back in the '70s there was no standard method for this. Enter Vint Cerf and Bob Kahn who developed the Internet Working Protocol. The internet is really a **design** philosohy and an architecture expressed in a set of protocols. <br>
Internet Protocol = IP = a computer's address e.g. 174:129:14:120 <br>
Visiting a website is really just your computer asking another computer for information. Your computer sends a message.

<img src="https://github.com/thequietlife/CTI-101/blob/824958a327a127181061da1b59e71d6551b551f3/images/IPv6.png"
alt="IP address showing all 32 bits" width="600"/>

<img src="https://github.com/thequietlife/CTI-101/blob/7fdbb82ea06368a55bef83e9af7d42e0aa8689dd/images/IP%204%20layers.png"
alt="IP broken down into layers" width="600"/>

<img src="https://github.com/thequietlife/CTI-101/blob/ac1590f45945f5628c353cda597c41b1b7ff7258/images/IPv6.png"
alt="breakdown of 128 bits of IPv6" width="600"/>

<img src="https://github.com/thequietlife/CTI-101/blob/9c5af5332fb2c077945a81aed3360c77f3a4d014/images/dns.png"
alt="pic shows how DNS works at a simplistic level" width="600"/>

<img src="https://github.com/thequietlife/CTI-101/blob/ba6cdb57bb7791664254f48403873730b8f4a215/images/fake.png"
alt="image shows DNS spoofing" width="600"/>

### Packets, Routing + Reliability

How is data delivered to you reliably?

<img src="https://github.com/thequietlife/CTI-101/blob/fd097bc0c835783c1826628db78d651307fc32fb/images/spotify%20server.png"
alt="image of laptop and spotify server" width="600"/>

Data travels on the internet in a much less direct way.

<img src="https://github.com/thequietlife/CTI-101/blob/6e3e5e1017e743138225fc0844212c1683b1c3d5/images/packets%20of%20info.png"
alt="image of packets of information travelling" width="600"/>

Packets of information <br>
A packet travels from one place to another kinda like when you try to wing it and take 3x longer to get somewhere than if you used a map. Many kinds of digital information can be sent with IP packets - but there are limits.

What happens when you build a rocket and need to move it to the launch pad? The rocket won't fit on one truck so it is delivered in parts.

<img src="https://github.com/thequietlife/CTI-101/blob/a9241762ff2153787005b4237ca4157c107d21b3/images/shuttle%20parts.png"
alt="image of space shuttle on a road" width="600"/>

When all the parts of the rocket have been delivered they are then assembled.

When you have a large image you want to share with a friend or upload to a website, that image may be made up of 10s of millions of bits, of 1s and 0s.

<img src="https://github.com/thequietlife/CTI-101/blob/6e3e5e1017e743138225fc0844212c1683b1c3d5/images/send%20more%20cat%20gifs.png"
alt="image of mobile and a picture of a cat" width="600"/>

There are too many to send in one packet. It will be broken down into 100s or 1000s of smaller parts called packets.

<img src="https://github.com/thequietlife/CTI-101/blob/6e3e5e1017e743138225fc0844212c1683b1c3d5/images/too%20many.png"
alt="cat gif zoomed in showing all the packets" width="600"/>

Routers act like traffic managers to keep packets moving through the networks smoothly. If one route is congested individual packets may travel different routes or even out of order.

<img src="https://github.com/thequietlife/CTI-101/blob/2c554566933e62b2cf6c08077d5658416c1d7ee7/images/routers.png"
alt="router and laptop with a network of routers in betweeon" width="600"/>

Every router keeps track of multiple paths for sending packets and it chooses the "cheapest" path available. Factors involved are time, politics, relatioships between companies. Often the best route isn't the most direct. <br>
**Fault Tolerant** Having options for paths makes the network fault tolerant. The network can keep sending packets even of something goes wrong.
<br> Basic key principle of the internet is **Reliability**.

### Transmission Control Protocol **TCP**
Responsible for making sure all your data gets delivered so that your spotify songs play without glitches.
Also referred to as **3-Way Handshake**.

<img src="https://github.com/thequietlife/CTI-101/blob/252c7db2e32a8497403f29e573468f4dd793d881/images/three%20way%20handshake.png"
alt="shows three way handshake, SYN, SYN/ACK, ACK" width="600"/> 

TCP manages the sending and receiving of all your data as packets. It's like a guaranteed mail service. TCP does a full inventory and sends back acknowledgements of each packet received. If all the packets are received, TCP signs for your delivery and the song plays.

If TCP finds some packets are missing it won't sign. Otherwise your song wouldn't sound as good or portions of the song could be missing. For each missing or incomplete packet, spotify will resend them. Once TCP verifies the delivery of the packets, for that one song, it will play.

TCP and router systems are scalable. They can work for 8 devices or 8 billion devices.

Principles of **Fault Tolerance Redundancy**, the more routers we add the more reliable the internet becomes. 

____

### The OSI Model

The Open Systems Interconnenction (OSI) Model is a universal language for computer networking. It is broken into seven parts to make it easier to understand and troubleshoot. It explains how different computer systems communicate with each other. It breaks down a complex topic into seven segments. Each layer has a specific job and communicates with the layers above and below.

The OSI model is used for understanding and troubleshooting networking problems. It provides a methodical approach. Issues can be pinpointed and fixed more efficiently.


| Number      | Layers   | Protocol data unit | Purpose | Troubleshooting |
| :---    |    :----:   |   ---    | -- | -- |
| 7 | Application | Data | Human + computer interaction | Check apps are properly configured |
| 6 | Presentation | Data | Makes data presentable for applications to consume. Encryption. Compressing data. Translation | Check for encryption issues |
| 5 | Session| Data | Communication. Responsible for opening and closing comms between two devices. Synchronises data transfer with checkpoints | Check if sessions are being maintained or if they are timing out |
| 4 | Transport | Segment | End-to-end communication between two devices (TCP and UDP happen). Includes firewalls |  Check port numbers. Use ```ping``` to see where connections are dropping  |
| 3 | Network | Packet | Data transfer between two different networks. Action central a lot happens here. Manages packet forwarding, routing and logical addressing (IP addresses) | Check IP addresses are configured correctly, routers working properly |
| 2 | Data link | Frame| Takes packets from the Network layer and breaks them into smaller pieces, frames | Check MAC addresses |
| 1 | Physical | Bit | Physical connection (cables, switches). Converts bits into a signal |  Start troubleshooting here first. Check power, cables, connections |








__________________
Sources: 
1. [Networking! ACK!, Julia Evans](https://jvns.ca/networking-zine.pdf)
2. [Why does DNS always break the internet?, InsiderPhD](https://youtu.be/yp1rH7Kj12o?si=fNMAa3lNEGPZpkAu)
3. [Understanding Basic Networking Concepts, Gerald Auger](https://youtu.be/XgOF6GhiMuM?si=rBbBhiCsdPO-1D4o)
4. [How The Internet Works, Code.org](https://www.youtube.com/playlist?list=PLzdnOPI1iJNfMRZm5DDxco3UdsFegvuB7)
5. [OSI model](https://en.wikipedia.org/wiki/OSI_model)
6. [What is the OSI Model?](https://www.cloudflare.com/en-gb/learning/ddos/glossary/open-systems-interconnection-model-osi/)
7. [OSI Model Layers and its Functions](https://electricalacademia.com/computer/osi-model-layers-functions/)

Credits:
1. Drawings made in Keynote and using [draw.io](https://app.diagrams.net/)
2. Icons from [Flaticon](https://www.flaticon.com/)
