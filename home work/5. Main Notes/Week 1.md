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

*To explain how internet travels we have two types of models*
1. OSI(Open systems intercommunications) model designed by ISO(International standadization organization) it is of 7-layers. it is just a frame work.
2. TCP/IP it is created by DARPA it is of 5 layers and it is real world application.

OSI 