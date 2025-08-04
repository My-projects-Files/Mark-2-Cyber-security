# Network And Network Security

## Network

It is a group of connected devices like phones, PC, Laptop etc. This devices can communicate over two types of network.
  - **Local Area Network (LAN)**
  - **Wide Area Network (WAN)**

**Local Area Network (LAN)** : A network that spans a small area like an office building, a school , (or) a home.

**Wide Area Network(WAN)** : A network that spans a large geographic area like a city, state, (or) Country.

## Common Devices in a Network:

**Hub** : A network device that broadcasts information to every device on the network.

**Switch** : A device that makes connection between specific devices on a network by sending and receiving data between them.

**Router** : A network device that connects multiple networks togethers.

**Modern** : A devices that Connets your router to the internet and brings internet access to the LAN.

**Virtualization tools** : Pieces of software that perform network opeations.

Webservice -> Moderm -> Firewall -> Router -> Switch -> Laptop

**Cloud Computing** : The Practice of using remote services applications, and network services that are hosted on the internet instead of an local physical devices.

**Cloud Network** : A Collection of service (or) computers that stores resources and data in remote data centers that can be accessed via the internet.

**Cloud Service Providers** : They office cloud computing to maintain applications 

  EX : On-demand Storage, Processing Power, Analytics

  They Provide three main categories of services.  
  - Software as a services (SAAS)
  - Infrastruction as a service (IAAS)
  - Platform as a Service (PAAS)

**Date Packet** : A Basic unit of information that travels from one devices to another within a network. Data packets includes instruction that tell the receiving devices what to do with the information. these instruction come in the form of a port number.  
  
  The data packet consists of
   
    |Header|_____Body_____|Footer|

Header --> IP address/MAC address/Protocol Number 
Body --> Message
Footer --> Indicates that message is Finished 

The Movement of data packets across a network can provide an indication how well the network is performing.
        
        Network performance can be mensured by bandwidth

**Band Width** : The amount of data a device receives every second. We can calculate bandwidth by dividing the quantity of data by the time in sec.

**Speed** : The rate at which data packets are received (or) downloaded. We need to check for both Speed & Bandwidth, because if either are irregular, it could mean an attack.

**Package Sniffing** : The Practice of capturing and inspecting data packets across a network.

## TCP/IP Module (Transmission control protocol / Interent protocol) 

TCP/IP is a standard model used for network communication.

**TCP(Transmission control protocol)** : An internet communication Protocol that allows two devices to form a connection and stream data.

**IP(Interent Protocol)** : A set of standards used for routing and addressing data pockets as they travel between devices on a network.

**Port** : A softwars based location that organizes the sending and receiving of data between devices on a network. Port number computer to split the network traffic & Prioritize the operations they will perform with the data.

Common Port are
        
        Port 25 --> Email
        Port 443 --> Secure internet communication
        Port 20 --> Large file Transfers

## TCP/IP Model

It is a Framework used to visualize. how data is organized and transmitted across the network.

Layers of the TCP/IP Model
  
  - Network Access Layer
  - Internet Layer
  - Transport Layer
  - Application Layer

**Network Access Layer** : It deals with creation of data packets and their transmission across a network. This includes hardware devices connected to physical cables & Switches that direct data to its destination.

**Internet Layer** : It is where ip adress are attached to data packets to indicate the location of the sender and receiver. It is also focuses on how network connect to each outher.

  EX : data packets containing info that determines whether they stay on the LAN (or) will be send to a remote network.

**Transport Layer** : It includes Protocols to control the flow of traffic across a network. these protocols permit (or) Deny communication with other devices and include info about the status of the connection.

**Application Layer** : Protocols determine how the data packets will interact with receiving devices. Functions that organized here includes file transfers and email services.

## The OSI Model :

It is the Standardized concept that describes the seven layers computers used to communicate and send data over the network.

            |_____ Application Layer___|
            |_____Presentation Layer___|
            |_____Session Layer________|
            |_____Transport Layer______|
            |_____Network Layer________|
            |_____Data Link Layer______|
            |_____Physical Layer_______|

## Interent Protocol (IP) address :

A Unique string of Characters that identifies the locaion of a device on the interent. Each device has an unique IP address.

There are of two types
  - IP Version 4 (IP V4)
  - IP Version 6 (IP V6)

### MAC address :
A unique alpanumeric identifier that is assigned to each physical device on the netwwork. MAC address tables are like a address book that the swith used to direct data packets to the appropriate device.

    EX :  MAC Address         Location on port
          0030c1-7fec40        A3
          0060b0-17de5b        A4

## Network Protocoles

A set of rules used by two (or) more devices on a network to describe the order of delivery and the strecture of the data.

### TCP Handshake:

TCP Versifies the connected devices before allowing any further communication to take place. This is called TCP Handshake. Once communication is established using a TCP handshake, a request is made to the network. the destination services will respond to that request and send data packets back.

**Address Resolution Protocol(ARP)** : A network protocol used to determine the MAC address of the next router (or) device on the path.

**HTTPS (Hyper text transfer Protocol secure)** : A network Protocol that provides a secure method of cmmunication between clients and website servers.

**DNS (Domain name service)** : A network protocol that translates internet dommain names into IP address.

**IEEE 802.11 (Institute of electrical and electronics engineers)** : It can also be called WIFI, A set of standards thet define communication for wireless LANs.\

**WIFI Protected Access (WPA)** : A Wireless Security Protocol for devices to connect to the interent.

**Wired Equivalent Privacy (WEP)** : It is a wireless security protocol designed to provide users with some level of privacy on wireless network as they have on wired.
