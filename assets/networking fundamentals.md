## Networking Fundamentals


### Summary: The OSI Model is a universal language for computer networking. It is broken into seven parts to make it easier to understand and troubleshoot. Start troubleshooting at Level 1 Physical.


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

### Protocols

* ARP
* BGP
* DNS
* Ethernet
* IP
* ICMP (ping)
* SSL/TLS
* UDP


### Other Concepts
* Checksum
* IP Address
* Nameserver
* NAT
* Socket
* Router
* TTL

  
* IP Addresses
* MAC Addresses

* Common Ports and Protocols

* Subnetting
* Routing
* Switching
  


[### Summary.]: # 


__________________
Sources: 
1. [Understanding Basic Networking Concepts, Gerald Auger](https://youtu.be/XgOF6GhiMuM?si=rBbBhiCsdPO-1D4o)
2. [OSI model](https://en.wikipedia.org/wiki/OSI_model)
3. [What is the OSI Model?](https://www.cloudflare.com/en-gb/learning/ddos/glossary/open-systems-interconnection-model-osi/)
4. [OSI Model Layers and its Functions](https://electricalacademia.com/computer/osi-model-layers-functions/)
5. 
