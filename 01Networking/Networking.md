Why Networking Matters
Ethical hacking is about understanding how computers communicate and where vulnerabilities exist in that communication.
Almost every attack—whether it's scanning ports, exploiting a server, intercepting traffic, or launching a web attack—relies on networking concepts.

Terminologies:
Hosts - any device that sends or receive traffic.
IP address - it is the identity of each hosts.
Repeaters - regenerate signals.
Hub - are simply multi-port Repeaters.
Switch - facilitate communication within network.(combination of hubs and bridges)
Router - facilitate communication between networks.
FireWall  - a secuirty device that montiors and controls network traffic based on defined rules.

Simple analogy:
Computers = Houses
IP addresses = House addresses
Data packets = Letters
Routers = Postal offices
Protocols = Delivery rules
Hackers = People trying to inspect or manipulate the mail.

What is a Network?
A network is a collection of devices connected together to exchange information and share resources.
Examples of devices:
Computers
Phones
Servers
Printers
IoT devices
Routers
Networks allow communication over cables or wireless connections.

LAN (Local Area Network)
A LAN is a network covering a small geographical area.
Examples:
Home Wi-Fi
School computer lab
Office network
Characteristics:
High speed
Usually privately owned
Devices are physically close together

WAN (Wide Area Network)
A WAN connects multiple LANs across large distances.
Examples:
The Internet
A company connecting offices in different cities
Bank branch networks

Characteristics:
Covers large geographical areas
Often uses infrastructure owned by ISPs
Usually slower than local communication
Think of a WAN as many LANs connected together.

IP Address
An IP (Internet Protocol) Address is a unique identifier assigned to a device on a network.
It tells data where it should be delivered.
Without IP addresses, computers wouldn't know where to send or receive information.

IPv4 vs IPv6
IPv4
Uses 32 bits.
Format: 192.168.1.1

Consists of four numbers separated by dots.
Maximum possible addresses:
About 4.3 billion
Problem:
The world has more devices than available IPv4 addresses.

IPv6
Uses 128 bits.
Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

Advantages:
Vastly larger address space
Better support for modern networking
Improved efficiency and scalability

        Comparison:
IPv4                                        IPv6
32-bit                                      128-bit
Dot-decimal notation           Hexadecimal notation
~4.3 billion addresses          Extremely large address pool
Becoming exhausted           Designed for future growth

MAC Address
A MAC (Media Access Control) Address is a hardware identifier assigned to a network interface.

Example: 00:1A:2B:3C:4D:5E
Unlike IP addresses:
MAC addresses identify the physical network adapter.
IP addresses identify a device's logical location on a network.
Think of it this way:
MAC Address → Who are you?
IP Address → Where are you?

Protocols
A protocol is a set of agreed rules for communication between devices.
Without protocols, computers would not understand each other.
Examples include:
TCP
UDP
HTTP
HTTPS
DNS
FTP

TCP (Transmission Control Protocol)
TCP provides reliable communication.
Features:
Checks that packets arrive correctly
Detects missing data
Requests retransmission if necessary
Maintains packet order
Imagine sending a 100-page document:
TCP ensures all 100 pages arrive and are assembled in the right order.
Common uses:
Websites
Email
File transfers
Banking applications

UDP (User Datagram Protocol)
UDP prioritizes speed over reliability.
Characteristics:
No guarantee of delivery
No packet ordering
No retransmission
If some data is lost, communication continues.
Common uses:
Video calls
Online gaming
Live streaming
Voice over IP (VoIP)

Comparison:
TCP                                        UDP
Reliable                                  Fast
Error checking                      Minimal overhead
Ordered delivery                  No ordering guarantee
Re transmits lost packets     Does not re transmit
Slightly slower                       Lower latency

DHCP (Dynamic Host Configuration Protocol)
DHCP automatically assigns IP addresses to devices joining a network.
Without DHCP:
Every device would need manual configuration.
With DHCP:
A device connects to the network.
It requests an IP address.
The DHCP server assigns one automatically.
That's why connecting to Wi-Fi usually works without manual setup.

DNS (Domain Name System)
Humans remember names more easily than numbers.
DNS translates domain names into IP addresses.
Example:
google.com
       ↓
142.250.x.x
Without DNS, you'd need to remember numeric IP addresses for every website.

Router
A router connects different networks and forwards traffic between them.
Functions:
Directs packets to their destinations
Connects your LAN to the Internet
Often provides DHCP services
Can include firewall and NAT functionality
Your home Wi-Fi router is the gateway between your local devices and the wider Internet.

Packet
Data sent across a network is broken into small units called packets.
Each packet typically contains:
Source address
Destination address
Payload (the actual data)
Control information
Large files are transmitted as many packets, which are reassembled at the destination.

Cloud Computing.
what is cloud computing?
It is the on-demand delivery of computing services—including servers, storage, databases, networking, software, and analytics—over the internet.

Core Benefits:
Cost Efficiency: Shifts IT costs from large upfront capital investments to flexible operational expenses.
Massive Scalability: Allows you to instantly add or remove computing power based on your current traffic spikes.
Global Access: Enables users to securely access files and applications from any device, anywhere in the world.
High Reliability: Offers built-in data backup, automated disaster recovery, and continuous hardware upgrades. 

Types of Cloud Deployments:
Public Cloud - Owned and run by third-party providers who deliver resources over the public internet to many companies.

Private Cloud - Infrastructure used entirely by one single business, often hosted in their own physical facility.

Hybrid Cloud - : Combines public and private clouds, allowing apps and data to share smoothly between them.

The Three Service Models:
Cloud services generally fall into three primary categories:
Infrastructure as a Service (IaaS): Renting raw infrastructure components like virtual servers and storage networks. Examples include Amazon Web Services (AWS) and Microsoft Azure Infrastructure. 

Platform as a Service (PaaS): Providers give you the hardware and software tools needed to build apps. You focus entirely on coding while the host manages operating systems and server maintenance.

Software as a Service (SaaS): Ready-to-use software applications delivered over a web browser. Examples include Google Drive, Netflix, and Microsoft Office 365.

Networking Tools and Attacks

MAC Address Spoofing.
It is the act of changing the factory-assigned Media Access Control (MAC) address of a network interface card (NIC) to a fake or stolen one. Every hardware device has a permanent, unique 12-digit physical fingerprint assigned at the factory, but operating systems allow users to temporarily mask it in software.

ARP Spoofing (ARP Poisoning)
It is a local network attack where a malicious actor sends falsified Address Resolution Protocol (ARP) messages onto a local area network (LAN) Information Security Reading Room. ARP is the protocol responsible for mapping a dynamic IP address to a physical MAC address on a local network.

Packet Capturing (Sniffing) 
It is the process of intercepting and logging data traffic passing over a computer network. When files, web pages, or messages travel across a network, they are broken down into small digital envelopes called packets.

OSI Model(Open systems Interconnection)
Different conmpanies provide a universal framework for networking.
Divides networking into 7 distinct, independent layer.
each layer has a specific job - communicates only with layers above/below.

1. Physical layer.
Transimission of raw bits over physical medium
No addressing at this layer - just electrical/optical/radio signals.
Security: Physical wiretapping and cable tapping happen at layer 1.

2. Data Link
Physical adressing using MAC address
Handles delivery within a single local network
Security: ARP spoofing, mac flooding and mac spoofing attacks

3. Network
Logical adressing - assigns and uses IP address
routing - determines the best path between networks
Security: IP spoofing - forging source IP to disguise attack origin

4. Transport 
End to End delivery of data between application
Manages PORT numbers - identifies which application gets the data
handles segmentation (breaking data) and reassembly
TCP & UDP
Secuirty: SYN flood attacks target TCP handshake

5. Session (conversation Manager)
Manages the sessions between two devices
Establish, maintains and terminates communication sessions
Handles session tokens
Security: Session Hijacking steals your session token to impersonate you

6. Presentation (data translator)
Translates data into a format both sides can UNDERSTAND
Handles: data encoding, compression and encrytion/decryption
TLS?SSL encryption and decryption happens here
Security: TLS stripping attacks target this layer - downgrading HTTPS to HTTp

7. Application
where users  and applications interact with the network
Provides network services directly to end-user applications Protocols: HTTP, HTTPS, DNS, FTP,SMTP,SSH,DHCP
Security: MOST attacks happen here - SQL injection, XSS, phishing, mawlare C2

Subnetting
It is the process of dividing a single large network into smaller, isolated sub-networks (called subnets).

Why Subnetting Matters.
Boosts Security: By splitting networks, you can isolate sensitive systems. For example, you can place a company's HR department on one subnet and guest Wi-Fi on another so guests cannot access payroll files.

Improves Performance: It limits network broadcast traffic. Instead of a device shouting a message to thousands of computers on a massive network, the noise is contained within a small subnet.

Saves IP Addresses: It prevents organizations from wasting limited IPv4 addresses by matching the network size precisely to the number of devices.



Key Takeaways for Ethical Hacking
Networking is the foundation of cybersecurity.
Every device communicating on a network has identifying information such as an IP address and often a MAC address.
LANs connect local devices, while WANs connect networks over large distances.
TCP emphasizes reliable delivery; UDP emphasizes speed.
DHCP automates IP address assignment.
DNS maps human-friendly names to IP addresses.
Routers move traffic between networks.
Data travels in packets governed by protocols.
