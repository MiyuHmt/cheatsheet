# Networks

## Networking topologies

Types of physical network topologies:

* Bus topology
* Star topology
* Ring topology
* Mesh topology
* Tree topology
* Hybrid topology

### Bus topology

Bus topology is a network type in which every computer and network device is connected to single cable. When it has exactly two endpoints, then it is called Linear Bus topology.

In the bus network topology, every workstation is connected to a main cable called the bus. Therefore, in effect, each workstation is directly connected to every other workstation in the network.

In the Cable required is least compared to other network topology.

### Star topology

In the star network topology, thiere is a central computer or server to which all the workstations are directly connected.
Every workstation is indirectly connected to every other through the central computer.

In this type of topology all the computers are connected to a single hub through a cable.

This hub is the central node and all others nodes are connected to the central node.

### Ring topology

It is called ring topology because it forms a ring as each computer is connected to another computer, with the last one connected to the first. Exactly two neighbours for each device.

In the ring network topology, the workstations are connected in a closed loop configuration. Adjacent pairs of workstations are directly connected.

Other pairs of workstations are indirectly connected, the data passing through one or more intermediate nodes.

### Mesh topology

It is a point-to-point connection to other nodes or devices. All the network nodes are connected to each other. Mesh has n(n-2)/2 physical channels to link n devices.

The mesh network topology employs either of two schemes, called full mesh and partial mesh. In the full mesh topology, each workstations is connected directly to each of the others.

### Tree topology

It has a root node and all other nodes are connected to it forming a hierarchy. It is also called hierarchical topology. It should at least have three levels to the hierarchy.

The tree network topology uses two or more star networks connected together.

The central computers of the star networks are connected to a main bus.

Thus, a tree network is a bus network of star networks.

### Hybrid topology

It is two different types of topologies which is a miniature of two or more topologies.

Unlike other networks, fault detection and troubleshooting is easy in this type of topology.

Its easy to increase the size of network by adding new components, without disturbing existing architecture.


## LAN Protocols

A network protocol defines rules and conventions for communication between network devices.

Protocols for computer networking all generally use packet switching techniques to send and receive messages in the form of packets.

### Types of LAN Protocols

* Ethernet
* Fast Ethernet
* Gig Ethernet
* WiFi
* FDDI
* ATM LANE

### Ethernet
The Ethernet protocol is by far the most widely used one. Ethernet uses an access method called CSMA/CD (Carrier Sense Multiple Access/Collision Detection).

This is a system where each computer listens to the cable before sending anything through the network.

Sometimes, two computers attempt to transmit at the same instant.

The Ethernet protocol allows for linear bus, star, or tree topologies.

### Fast Ethernet

Ethernet is the most ubiquitous local area networking protocol and utilizes copper ethernet cables (Cat3, Cat5, 
Cat5e and Cat6), fiber optics, or wireless (WiFi) connections to an ethernet switch or wifi router.

Fast Ethernet is a local area network (LAN) transmission standard that provides a data rate of 100 megabits per second (referred to as "100BASE-T").

Workstations with existing 10 megabits per second (10BASE-T) Ethernet card can be connected to a Fast Ethernet network.

### Gig Ethernet

Gigabit Ethernet, a transmission technology based on the Ethernet frame format and protocol used in local area 
networks (LANs), provides a data rate of 1 billion bits per second (one gigabit).

Gigabit Ethernet is defined in the IEEE 802.3 standard and is currently being used as the backbone in many enterprise networks.

Gigabit Ethernet is carried primarily on optical fiber (with very short distances possible on copper media).

### WiFi

WiFi, or "Wireless Fidelity" is a descriptive acronym for describing the use and implementation of 802.11 wireless local area networking protocols (WLAN).

If you connect to your internet at home using a wireless network, or connect to a WiFi network at say a coffee shop, a airport, you have undoubtedly used 802.11 technology.

Wireless Local Area Networking devices use frequencies in the microwave range as a medium to encapsulate data onto.

### FDDI

FDDI utilizes fiber optic technology as the communications media.

FDDI transmits light through glass or clear plastic strands that are thinner than a human hair.

These strands carry signals from place to place and are connected to laser-light emitters.

The strands are lit and unlit to provide data communication. This makes FDDI very expensive however, and so you rarely see it in a computer LAN.

### ATM LANE

Asynchronous Transfer Mode (ATM) is a network protocol that transmits data at a speed of 155 Mbps and higher.

ATM works by transmitting all data in small packets of a fixed size; whereas, other protocols transfer variable length packets.

ATM supports a variety of media such as video, CD-quality audio, and imaging. ATM employs a star topology, which can work with fiber optic as well as twisted pair cable.

ATM is most often used to interconnect two or more local area networks.


## WAN Protocols

The acronym WAN is used to refer to networks spanning much areas larger than a LAN does and often include circuits provided by a telecommunications carrier or a private leased line.

Protocols that can transmit across longer distances measured in miles or kilometers are used to build WANs.

### Types of WAN Protocols

* X.25
* Frame Relay
* ISDN
* DSL

### X.25

The X.25 protocol, adopted as a standard by the Consultative Committee for International Telegraph and Telephone (CCITT), is a commonly-used network protocol.

The X.25 protocol allows computers on different public networks (such as CompuServe, Tymnet, or a TCP/IP network) to communicate through an intermediary computer at the network layer level.

X.25's protocols correspond closely to the data-link and physical-layer protocols defined in the Open Systems Interconnection (OSI) communication model.

### Frame Relay

Frame Relay is scalable WAN solution that is often used as an alternative to leased lines prove to be cost unaffordable.

With Frame Relay, you can have a single serial interface on a router connecting into multiple remote sites through virtual circuits.

AT&T stopped offering frame relay in 2012 but said it would support existing customers until 2016.

### ISDN

The Integrated Services Digital Network was the first telecommunications service designed specifically for digital data communication

ISDN was designed to run over standard voice digital telephone systems already in place

Consequently ISDN conforms to specifications found in the telecom's digital voice network.

However, it took so longer for ISDN to be standardized that it was never fully deployed in the telecommunications networks it was intended for.

### DSL

DSL (Digital Subscriber Line) is a technology for bringing high-bandwidth information to homes and small businesses over ordinary copper telephone lines.

xDSL refers to different variations of DSL, such as ADSL, HDSL, and RADSL.

DSL technology uses normal phone line technology to send digital signals to the DSL modem.

One of the major advantages of DSL over Cable Modems is that the line is not shared to the Central Office; however, the slow connections are rarely associated with this segment of your connection.

## Network Devices

Computer networking devices are units that mediate data in a computer network and are also called network equipment. Units which are the last receiver or generate data are called hosts or data terminal equipment.

### Types of Network Devices

* HUB
* Switches
* Routers
* NICs

### HUB

Networks using a Star topology require a central point for the devices to connect

Originally this device was called a concentrator since it consolidated the cable runs from all network devices. The basic form of concentrator is the hub

The hub is a hardware device that contains multiple, independent ports that match the cable type of the network.

Most common hubs interconnect Category 3 or 5 twisted-pair cable with RJ-45 ends, altough Coax BNC and Fiber Optic BNC hubs also exist.

### Switches

Switches are a special type of hub that offers an additional layer of intelligence to basic, physical-layer repeater hubs.
A switch must be able to read the MAC address of each frame it receives.

This information allwos switches to repeat incoming data frames only to the computer or computers to which a frame is addressed. This speeds up the network and reduces congestion.

Switches operate at both the physical layer and the data link layer of the OSI Model.

### Routers

Routers are networking devices used to extend or segment networks by forwarding packets from one logical network to another.

Routers are most often used in large internetworks that use the TCP/IP protocol suite and for connecting TCP/IP hosts and local area networks (LANs) to the internet dedicated leased lines.

Routers work at the network layer (layer 3) of the OSI reference model for networking to move packets between networks using logical addressses (wich, in the case of TCP/IP, are the IP addresses of destination hosts on the network).

### NICs

Network Interface Card, or NIC is a hardware card installed in a computer so it can communicate on a network.

The network adapter provides one or more ports for the network cable to connect to, and it transmits and receives data onto the network cable.

Every networked computer must also have a network adapter driver, which controls the network adapter.
Each network adapter driver is configured to run with a certain type of network adapter.

## Concepts of IP

If a device wants to communicate using TCP/IP, it needs an IP address.

Whan the device has an IP address and the appropriate software and hardware, it can send and receive IP packets.

Any device that can send and receive IP packets is called an IP host.

IP addresses consist of a 32-bit number, usually written in dotted-decimal notation.

## Packets and addresses

### Addresses

A packet is the basic unit of information in network transmission.

Most networks use TCP/IP as the network protocol, or set of rules for communication between devices.

They fit into the standard model of networking model, known as the OSI model.

The structure of packets and packet-switching networks allow for fast and reliable data transmission, and make networks like the internet possible.

### Packets

An IP address is an address used in order to uniquely identify a device on an IP network.

The address is made up of 32 binary bits, which can be divisible into a network portion and host portion with the help of subnet mask.

The 32 binary bits are broken into four octets (1 octet = 8 bits)

Each octet is converted to decimal and separated by a period (dot).

## IP service port

The service-port interface controls communications through and is statically mapped by the system to the service port.

The service port can obtain an IPv4 address using DHCP, or it can be assigned a static IPv4 address.

But a default gateway cannot be assigned to the service-port interface.

The default gateway cannot be assigned to the service-port interface.

## Internet Protocol (IP)

The Internet Protocol is the method or protocol by which data is sent from one computer to another on the internet.

Each computer (known as a host) on the internet has at least one IP address that uniquely identifies it from all other computers on the internet.

IP by itself is something like the postal system.

Most networks combine IP with a higher-level protocol called TCP

## Address classes

Internet Protocol hierarchy contains several classes of IP Addresses.

To be used efficiently in various situations as per the requirement of hosts per networks.

The IPv4 addressing system is divided into five classes of IP addresses.

All the five classes are identified by the first octet of IP address

### Class A address

The first bit of the first octet is always set to 0.

Thus the first octet ranges from 1 - 127, i.e.

Class A addresses only include IP starting from 1.x.x.x to 126.x.x.x only

The IP range 127.x.x.x is reserved for loopback IP addresses

### Class B address

An IP address which belongs to class B has the first two bits in the first octet set to 10.

Class B addresses range from 128.0.x.x to 191.255.x.x

The default subnet mask for class B is 255.255.x.x

Class B has 16384 (2^14) network addresses and 65534 (2^16-2) host addresses.

### Class C address

The first octet of class C IP address has its first 3 bits set to 110.

Class C addresses range from 192.0.0.x to 223.255.255.x

The default subnet mask for class B is 255.255.255.x

Class C gives (2^21) network addresses and 254 (2^8-2) host addresses.

### Class D address

Very first four bits of the first octet in class D IP addresses are set to 1110.

Class D has IP address range from 224.0.0.x to 239.255.255.255

Class D is reserved for multicasting.

Host address from the IP address, and class D does not have any subnet mask.

## TCP (Transmission Control Protocol)

TCP is a network communication protocol designed to send data packets over the internet.

TCP/IP is a set of rules (protocols) governing communications among all computers on the Internet.

TCP/IP is a combination of 2 separate protocols: TCP and IP.

### Three most common TCP/IP protocols

* HTTP
* HTTPS
* FTP

### HTTP

HTTP - used between a web client and a web server, for non-secure data transmissions.

A web client (i.e. Internet browser on a computer) sends a request to a web server to view a web page.

The web server receives that request and sends the web page information back to the web client.

### HTTPS

HTTPS - used between a web client and a web server, for secure data transmissions.

Often used for sending credit card transaction data or other private data from a web client (i.e. Internet browser on a computer) to a web server.

HTTPS provides authentication of the website and associated web server with which one is communicating.

### FTP (File Transfer Protocol)

FTP uses the Internet's TCP/IP protocols to enable data transfer.

Used between two or more computers.

One computer sends data to or receives data from another computer directly.

FTP uses a client-server architecture, often secured with SSL/TLS.

### UDP (User Datagram Protocol)

User Datagram Protocol (UDP) is a transport layer protocol defined for use with the IP network layer protocol.

It is defined by RFC 768 written by John Postel.

UDP provides a minimal, unreliable, best-effort, message-passing transport to applications and upper-layer protocols.

UDP and its UDP-lite variant are unique in that they do not establish end-to-end connections between communicating end systems.

### ICMP (Internet Control Message Protocol)

ICMP is an error-reporting protocol network devices like routers use to generate error messages to the source IP address when network problems prevent delivery of IP packets.

It is an extension to the Internet Protocol defined by RFC 792.

ICMP messages generated by router R1, in response to message sent by H0 to H1 and forwarded by R0.

### DNS (Domain Name System)

Internet service that translates domain names into IP addresses.

Because domain names are alphabetic, they're easier to remember.

The DNS system is, in fact, its own network.

If one DNS server doesn't know how to translate a particular domain name, it asks another one, and so on, until the correct IP address is returned.
