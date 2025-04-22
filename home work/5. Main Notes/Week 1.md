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
- Gopher : This protocol is used to transfer documents over network.
- Simple network management protocol : It manages the exchange of data between network between devices

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

*Client* : Workstations.
*Server* : It has more resources which clients use.
*Network devices*
1. *Repeater* : It is a hardware device which regenerates and amplifies incoming signals which will boost the networking distance.
2. *Hubs* : It is a networking component which connects all devices and sends the data to all devices weather the device needs it or not and acts as a repeater. if two devices talks at once you will get a crash. it is also called as multiport repeater.
3. *Transceiver* : it is a device which is capable of sending and grabbing data.
4. *Network interface card(NIC)* : It acts as a gateway between computer and a network. Its what allows the computer to communicate with a network. It operates at data link layer.
5. *Bridges* : A networking devices which allows to connect two or more local area networks to make a larger network. it operates at data link layer. it is a smarter hub. it filters traffic based on mac address. but using one bridge we can only connect two local area networks.
6. *Switches* : Its a networking devices which allows to connect two or more devices within a network and it will send to only one who needs it. it is a layer two device. But some devices hits layer 3. it is also called as multiport bridge.
7. *Routers* : It allows to send data to different networks. and its also capable of finding the nearest path. it works at level 3. it can ping across different networks.
Hubs->Bridges->Switches->Routers.

## *Switching networks* 

*Switching a network means to switch between from one node to other node while transferring data from source to destination*

There are two types of *Switching technologies*
### *Circuit Switching*

It is a networking method where a physical or dedicated path is setup between devices for whole conversation.

There are three phases for this method
1. *Establish* : when its start, the network finds and reserve the nearest path through switching nodes.
2. *Transfer* : once the path is found the data will flow continuously till the transmission is completed.
3. *Disconnect* : When the transmission is completed the path is freed so other devices can use that path.
Must have switching capacity and channel capacity to establish connection.
Must have intelligence to workout routing.

There are four approaches to this.
#### *Space-Division switch*

it will find one cross-point in a matrix of node and it will establish a path, uses it until its done.
#### *Time Division switch*

The switch divides signals into fixed time interval, assigning each connection its own slot
#### *TDM Bus*

Time division multiplexing bus same as time division switch.
### *Packet Switching*

It is a efficient method which will chops the data into small chunks and sends it to the destination and after that it will reassemble the received packages. These small chunks called packets. 

There are three steps for this.
1. *Data chop* : The data gets splits into packets. Each with a header and payload.
2. *Independent routing* : Each packet takes it own path through switching nodes.
3. *Reassembly* : The destination device keeps back the packets together using sequence number.

there are two approaches
#### *Datagram approach* 

Packets will send from transmitter and it is up to receiver to receive the packets and rearrange in order. Packets may gets lost.
#### *Virtual circuit approach*

This approach will set a virtual path just like circuit switching but software sets its path, and each packet has virtual circuit identifier which tells the packet to take which route.

### *Network Protocols*

*Key elements of a protocol*

1. Data format.
2. Signal level.
3. Control information.
4. Error handling.
5. Speed matching.
6. Sequencing.

[[OSI model]]


