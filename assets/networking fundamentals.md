## Networking Fundamentals

### What is the Internet? 

The internet is a network of networks. It links billions of devices together all around the globe.

### How does the Internet Work?

If you are in a cafe using wifi, the bits get sent through a wireless router and then are transformed to the physical wire to travel the really long distances of the internet. The physical method for sending bits may change in the future. e.g. lasers sent between satellites or radio waves from balloons or drones. But the binary representation of information and protocols for sending that information and receiving that information have pretty much stayed the same.

### Bit Sending

Everything on the internet - emails, cat videos - all come down to these ones and zeros being delivered by electronic pulses, light beams, radio waves

### IP Addresses + DNS

Networks need to be able to talk to one another. Back in the '70s there was no standard method for this. Enter Vint Cerf and Bob Kahn who developed the Internet Working Protocol. The internet is really a **design** philosohy and an architecture expressed in a set of protocols. <br>
Internet Protocol = IP = a computer's address e.g. 174:129:14:120 <br>
Visiting a website is really just your computer asking another computer for information. Your computer sends a message.

<img src="https://github.com/thequietlife/CTI-101/blob/824958a327a127181061da1b59e71d6551b551f3/images/IPv6.png"
alt="IP address showing all 32 bits" width="600"/>



### Summary
The OSI Model is a universal language for computer networking. It is broken into seven parts to make it easier to understand and troubleshoot. Start troubleshooting at Level 1 Physical.


### The OSI Model

The Open Systems Interconnenction (OSI) Model is a universal language for computer networking. It explains how different computer systems communicate with each other. It breaks down a complex topic into seven segments. Each layer has a specific job and communicates with the layers above and below.

The OSI model is used for understanding and troubleshooting networking problems. It provides a methodical approach. Issues can be pinpointed and fixed more efficiently.


| Number      | Layers   | Protocol data unit | Purpose | Troubleshooting |
| :---    |    :----:   |   ---    | -- | -- |
| 7 | Application | Data | Human + computer interaction | Check apps are properly configured |
| 6 | Presentation | Data | Makes data presentable for applications to consume. Encryption. Compressing data. Translation | Check for encryption issues |
| 5 | Session| Data | Communication. Responsible for opening and closing comms between two devices. Synchronises data transder with checkpoints | Check if sessions are being maintained or if they are timing out |
| 4 | Transport | Segment | End-to-end communication between two devices (TCP and UDP happen). Includes firewalls |  Check port numbers. Use ```ping``` to see where connections are dropping  |
| 3 | Network | Packet | Data transfer between two different networks. Action central a lot happens here. Manages packet forwarding, routing and logical addressing (IP addresses) | Check IP addresses are configured correctly, routers working properly |
| 2 | Data link | Frame| Takes packets from the Network layer and breaks them into smaller pieces, frames | Check MAC addresses |
| 1 | Physical | Bit | Physical connection (cables, switches). Converts bits into a signal |  Check power, cables, connections |








__________________
Sources: 
1. [Networking! ACK!, Julia Evans](https://jvns.ca/networking-zine.pdf)
2. [Why does DNS always break the internet?, InsiderPhD](https://youtu.be/yp1rH7Kj12o?si=fNMAa3lNEGPZpkAu)
3. [Understanding Basic Networking Concepts, Gerald Auger](https://youtu.be/XgOF6GhiMuM?si=rBbBhiCsdPO-1D4o)
4. [OSI model](https://en.wikipedia.org/wiki/OSI_model)
5. [What is the OSI Model?](https://www.cloudflare.com/en-gb/learning/ddos/glossary/open-systems-interconnection-model-osi/)
6. [OSI Model Layers and its Functions](https://electricalacademia.com/computer/osi-model-layers-functions/)


