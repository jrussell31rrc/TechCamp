### Red River College's Applied Computer Education Department presents  
## Tech Camp
# Part 3: Networking

### Keeping You Connected To The Things That Matter

### Introduction
We all use the Internet daily for many things.  What do you use it for?
Research
- Education
- Shopping
- Phone Calls
- Instant Messaging
- Meetings
- GPS
- Gaming
- Tech Camp today

Networks provide the underlying communications paths that the Internet run on.  All communication must take place over some sort of media.  

Using the internet perhaps by connecting to a web site may involve many different types of media.  
<img src="0 - Images/03 Networking 3_1.png" alt="Different types of physical media can be used to communicate">

| Media Types | Description |
| - | - |
| Metal wires within cables | Uses Electrical Impulses |
| Glass or plastic fibers within cables (fiber-optic cable) | Uses pulses of light |
| Wireless transmission | Uses modulation of specific frequencies of electromagnetic waves |

Each type of media uses different methods for communication.  Copper cables (Ethernet or co-ax) use electrical impulses to send data.  Fiber-optic cables uses pulses of light.  Wireless transmission is accomplished through modulation of specific frequencies of electromagnetic waves.  Regardless of the media, all transmissions are sent as binary (ones and zeroes) either on or off. So when using fiber optic – the light is either on or off (1 or 0).

Using the internet for house by connecting to a website may involve many different types of network media. Imagine many networks connected by various media types, copper, fiber, or wireless, that expand across the world. This is the start to understanding how we are all connected through the internet.
<img src="0 - Images/03 Networking 4_1.png" alt="Connecting to a Website with media type examples">

### Typical home network setup.
Within our typical home network, we have internal media which may be wireless and/or Ethernet.  Our Internet Service Provider, or ISP, provides us with hardware and a connection to their service.  That connection can be fibre optic, co-ax cable, through satellites, or plain old telephone service.
<img src="0 - Images/03 Networking 5_1.png" alt="Typical Home Network Setup">

Their equipment provides your home network with a DHCP server, a gateway and NAT.  A DHCP server provides logical addresses to any powered-on device.  The gateway provides the device with an address to get off of the network and out to the Internet.  The NAT (Network Address Translation) will translate our private address into a public address which will allow that information to go out onto the Internet.  Private internal addresses are not allowed on the internet and were designed to expand the address space of IPv4.  The ISP hardware also provides a switching function where the device will convert the internal communication protocols into the required protocol to go out to the Internet.

### Importance of standards
Standards are set and enforced for all network communication.  To understand the reason we need to learn a little about the history of the computer industry. Not long ago, Companies like IBM and Digital Equipment Corporation (DEC) were the leading computer manufacturers in the world manufactured devices which were not compatible with each other. So if you bought a computer from IBM you had to buy a monitor, printer and everything else from IBM. There were many companies that bought equipment from both equipment manufacturers but the problem was the devices could not communicate with each other. That was about the time when international organization for standards or more commonly known as ISO thought that there was a need for a standard.  Now all devices and communications adhere to standards meaning equipment can work seamlessly together and devices from all different manufacturers can communicate.

- We have seen that internet communication takes place in a variety of ways
- This leads to the importance of standards in the networking world
- In order to provide seamless communication, all networking media and the transmission of that communication follows protocols
- Networking protocols can be defined as rules that govern the transmission of data

### We have all sorts of acronyms in the networking world. Some you may recognize.
<img src="0 - Images/03 Networking Presentation 07.png" alt="Acronym Stew - many networking acronyms are pictured">
IPv4 – Internet Protocol version 4
IPv6 – Internet Protocol version 6
TCP – Transport Control Protocol
UDP – User Datagram Protocol
DNS – Domain Name Service  
DHCP – Dynamic Host Configuration Protocol
Http – hypertext transfer protocol
Https – secure hypertext transfer protocol

#### Analogy for network communication
If you were to mail a letter, you are required to perform certain tasks and to provide information in a standard format.  You would provide the address of the recipient on the front of the envelope.  You would usually put your address in the top left-hand corner of the envelope so that the recipient knows where the letter came from.  You would also put a stamp in the top right-hand corner of the envelope.  By performing these tasks and conforming to the standards, you would assume your letter would move through the postal system and would be successfully delivered.  Like a letter, certain pieces of information are required for any network communication to take place. The three required pieces are MAC address, logical address and port number.
<img src="0 - Images/03 Networking 9_1.png" alt="Addressing on a physical letter">
<img src="0 - Images/03 Networking 9_2.png" alt="Letter addressing as network addresses example">


### Requirements for communication
In order to communicate between your device and any other device on the network three pieces of information are needed:
  - MAC address
  - Logical address – IPv4 or IPv6
  - Port number

We will explore each of these pieces of information and see how they work together to deliver information over the Internet

### MAC Addresses
Your computer's Network Interface’s physical address.
Is like your name... stays the same even if you move to a different street.
"Burned in" by the manufacturer into the device. Unique for every device
Some operating systems are offering the option of randomizing your MAC address as a security feature
Displayed as a hexadecimal number
The MAC address is made up of 6 pairs of hexadecimal numbers separated by either a dash ('-') or a semi-colon (':')

A MAC address is a physical address of the network interface. Also known as a Network Interface Card (NIC). You can look at your MAC address in a variety of ways.  MAC addresses are unique.  Some operating systems will allow you to randomize your MAC address as a security feature, like your smart phone.

#### Try it out
From the settings of an iPhone, we can select our Wi-Fi network and then select the little 'i' beside the name. You should see a Private Address slider. When you turn that off, you will see the true MAC address of your wireless network interface card on your iPhone. Be sure to turn the slider back on to keep your device anonymous on untrusted networks.

### IP Addresses
IP Address – can be ipv4 or ipv6.  Most devices will have both addresses as IPv4 is reaching its end-of-life and we will be moving to IPv6.

Your computer’s Logical Address
Like a street address
Packets are sent addressed to a specific “house/host” which is located on a specific “street/network”
Routers read packets and send them in the direction toward the network the packet is addressed to.

#### Examples

<img src="0 - Images/03 Networking 26_1.png" alt="IPv4 address example">
IPv4 - 192.168.100.108

<img src="0 - Images/03 Networking 27_1.png" alt="IPv6 address example">
IPv6 - fe80::152e:fb67:e18a:b2ec

### Many ways to determine the address of my device
Every device will have the required addresses for network communication
Depending upon your operating system and the access you are granted on the device, there are different ways to determine the address of your device
The following slides will demonstrate methods to find your address on different devices
Choose the method that matches both your operating system and the access you have to the device settings

#### Well known port numbers
| Port Number | Protocol | Application |
| 20​ | TCP​ | File Transfer Protocol (FTP) - Data​ |
| 21​ | TCP​ | File Transfer Protocol (FTP) - Control​ |
| 22​ | TCP​ | Secure Shell (SSH)​ |
| 23​ | TCP​ | Telnet​ |
| 25​ | TCP​ | Simple Mail Transfer Protocol (SMTP)​ |
| 53​ | UDP, TCP​ | Domain Name Service (DNS)​ |
| 67​ | UDP​ | Dynamic Host Configuration Protocol (DHCP) - Server​ |
| 68​ | UDP​ | Dynamic Host Configuration Protocol - Client​ |
| 69​ | UDP​ | Trivial File Transfer Protocol (TFTP)​ |
| 80​ | TCP​ | Hypertext Transfer Protocol (HTTP)​ |
| 110​ | TCP​ | Post Office Protocol version 3 (POP3)​ |
| 143​ | TCP​ | Internet Message Access Protocol (IMAP)​ |
| 161​ | UDP​ | Simple Network Management Protocol (SNMP)​ |
| 443​ | TCP​ | Hypertext Transfer Protocol Secure (HTTPS)​ |

### DNS
DNS – maps names to ip addresses.  Without a DNS service we would have to remember the IP address for every web site we wanted to visit.

- Domain Name Services (DNS) are used to map names to IP addresses.
- DNS uses both TCP and UDP port numbers
- Without this service, we would have to enter the numeric address of every device we wanted to communicate with.
- Both Windows and Linux use versions of the nslookup utility enable user DNS queries.

Use the **nslookup** command in one of the following applications:
- Command Prompt, on Windows
- Terminal Application, on Macintosh
- on Linux, you would use **dig**  Open browser & access via ip address.

 Type this command then press enter/return:
```
 nslookup rrc.ca
```

It reveals the server's ip address associated with rrc.ca

Now, try this. Type this command then press enter/return:
```
nslookup 35.182.194.48
```

#### Let's try it in your Goorm container
From your goorm container, type in terminal and press enter:
```
apt update
```

Type in terminal and press enter:
```
apt install dnsutils –y
```

Now try typing in terminal and press enter:
```
nslookup rrc.ca
```

### Viewing a website
To view a web site you will use a URL (Universal Resource Locator) or an ip address
Your device has to have access to a DNS server in order to use a URL
<img src="0 - Images/03 Networking 36_1.png" alt="Chrome Logo">
<img src="0 - Images/03 Networking 36_2.png" alt="Firefox Logo">
<img src="0 - Images/03 Networking 36_3.png" alt="MS Edge Logo">
<img src="0 - Images/03 Networking 36_4.png" alt="Explorer Logo">
<img src="0 - Images/03 Networking 36_5.png" alt="Safari Logo">

### Firewalls
- Firewalls are a set of rules on a computer or network device that determine what type of communication is allowed or denied
- Rules can filter communication by port number, IP address or MAC address
- These rules may be set by your organization therefore you may not have access to make changes
- By default, firewalls are configured to block everything coming in (implicit deny) except the items on its exception list (items going out are unaffected)

#### Firewalls – Port forwarding
- Port Forwarding allows remote devices access through your firewall to a specific IP address and  port number(s) inside your LAN.
- Use caution when configuring port forwarding rules as you may be exposing your device to untrusted networks (e.g. Internet).

#### Try it out
In Goorm, from the top navigation menu, choose: **Container**, then **Port Forwarding Configuration**
1. Set the Internal Port number to: **80**
1. Click the **Register** button
1. Copy the address under **Command**. The format should look similar to this: 542.218.62.176:50418
1. Paste the address into your search bar in your browser.

#### Try out

# TODO: add try-it-out commands for Goorm

# TODO: remove unused information
DHCP - Will assign an address to a device from a group of available addresses.  This can be configured by the administrator.

Gateway - is the router port that will allow you to get off the internal network and access another network or the internet.  In your home network this is the typically the device provided by the ISP.

How to find this information?  Each device is different.  The Powerpoint presentation provides screenshots to help you find all of your address information on various devices.  Can you find your information on your goorm container?  On your phone?  On your device?

Port number – used to identify the application required.  There are well-known port numbers which identify certain applications such as http (80) or https (443).  A port number can be any number between 0-65535.



Goorm Container Setup Commands
apt install tshark -y
usermod -a -G wireshark root
newgrp wireshark
chgrp wireshark /usr/bin/dumpcap
apt install dnsutils -y
