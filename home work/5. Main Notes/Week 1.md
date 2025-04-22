*Network Architecture* is a visualizing how networking components talks to each other.

*Protocol* is a controlled sequence of messages that is exchanged between two or more systems to complete a given task.
## *Protocol Stack*

1. *Physical layer* : convert digital data into analog signal or vice versa.
2. *Data link layer* : it will ensure all the devices accessing the data properly.
3. *Network layer* : It will finds the easy path to transfer data.
4. *Transport layer* : It will control the traffic of the network.
5. *Application layer* : It will provide a user interface for the user to interact with network.

### *protocols at different layers*

*Physical layer* : Ethernet (IEEE 802.3), WIFI (IEEE 802.11) works here but not too much.
*Data link layer* : Ethernet, WIFI, Bluetooth, UMTS(Universal Mobile Telecommunications System (3G Network bro)), LTE(Long term evolution).
*Network layer* : IPV4 it is a 32bit it has 4.3 billion address to locate, IPV6 is a 128 bit it has Trillions of address to locate. MPLS (Multi-protocol label switching) is a technique used to route and direct traffic that uses labels instead of addresses to handle data flow from one router to another.
*Transport layer* : *Transfer control protocol(TCP)* reliable protocol it ensures the data is transferred completely it is three way hand shake(SYN,SYN-ACK,ACK). *UDP(User datagram protocol)* it is designed for speed and efficiency. It does not guarantee the data transfer. *Real time transport protocol (RTP)* used for delivering audio and video over IP addresses, like streaming and video conferences.
*Application layer* : HTTP(Hyper text transfer protocol) for websites, FTP(File transfer protocol) for files over network, SMTP(simple mail transfer protocol) for sending and receiving mails.

*More protocols*
- POP3 - post office protocol version 3 used to retrieving emails from a message server to a local device.
- IMPA4 - Internet Message Access Protocol version 4 same as "POP3".
- TELNET - It allows text based communication between user and client.
- Trivial File Transfer protocol - It allows to transfer files between server and client.
- BOOTP - Bootstrap protocol it will automatically configure devices with an IP address especially in initial booting process. it is a part of DHCP (Dynamic host configuration protocol).
- ARP (Address resolution protocol) : it binds IP address and mac address together.
- ICMP (Internet control message protocol) : It is used to report errors while transferring data.

*To explain how internet travels we have two types of models*
1. OSI(Open systems intercommunications) model designed by ISO(International standardization organization) it is of 7-layers. it is just a frame work.
2. TCP/IP it is created by DARPA it is of 5 layers and it is real world application.

*[[OSI model]]*

*TCP/IP protocol*

1. *Application layer* : it is used to interact with user and collect the data from the user using different types of protocols like telnet, ftp, http.. etc.
2. *Transport layer* : Here TCP and UDP protocols acts and adds the app header info like source and destination ports, sequence numbers for reliability for TCP. UDP is lighter just ports and length it is fast but unreliable. 
3. *Network layer* : This layer adds IP header for source and destination to transfer data, and it adds one TCP header. Here protocols like ARP and ICMP. it is like GPS to our data.
4. *Ethernet layer* : it adds ethernet header and trailer which is used for CRC for error checking.
5. *Physical layer* : This physical layer turns data into electrical signal, radio waves and all. Nothing is added here just transmission.

### *Local area network(LAN)*

