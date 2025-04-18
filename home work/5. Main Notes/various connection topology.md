
2025-04-17 21:54

Topic: 

Tags: 

## *Reference*



---

## *Network Topology*

A network topology is a structure or organization of devices connect in a network.
There are 8 types of topologies:- 
### *Bus topology*

![[Pasted image 20250417235820.png]]

A single cable is connected to every device and make a network. Data travels through this cable. The ends need terminator to stop from bouncing back. If terminators are not there in ends devices get the same data again and again so we need terminators.

Its Advantages are cheap and good for small networks.
Disadvantages are if one devices get malfunctioned or disconnected whole network will be off.


### *Star topology*

![[Pasted image 20250418001828.png]]

In this star topology all devices are connected to only one hub through its own cable. Data goes to hub to reach its destination.
Its advantages are if any cable disconnects the individual device gets effected not the whole system like bus topology.
its disadvantages are if hub dies then the whole network stops. It needs more cables than bus topology.


### *Ring topology*

![[Pasted image 20250418223239.png]]
In ring topology every device connects to its next device forming a ring. Data travel in one direction or in both directions (in dual-ring setups).
Its advantage is Equal access for all devices.
Its disadvantages are if one device dies whole network gets affected, and it is very tricky to add a device to this network.


### *Mesh topology*

![[Pasted image 20250418224543.png]]

In mesh topology every device is connected to every other device making it reliable. For n devices n(n-1)/2 connections will be there.
Its advantages are it is super reliable meaning no single failure can stop the flow of network.
Its disadvantages are it is messy a lot, it needs more cables to connect and adding a network is super hard.


### *Tree topology*

![[Pasted image 20250418230254.png]]

In tree topology a root node (router) connects to sub nodes (switch) and it connects to more devices and so on.. it is hierarchical data flows up to down and down to up. The root link branches and branches links to leaves.
Its advantages are it is good for large networks and it is easy to add a new device.
Its disadvantages are it requires lot of wiring and it will make you tiring. if root fails then RIP network.


### *Hybrid topology*

![[Pasted image 20250418231819.png]]

Hybrid topology mixes two or more topologies to meet certain specifications and needs.
Its advantages are flexible, customizable and scalable. we can upgrade parts without rebuilding everything.
Its disadvantages are complex to design and build and needs lot of wiring. it costs more and troubleshooting is tricky.


### *Point to point*

![[Pasted image 20250418233155.png]]

In this topology two devices connected directly through a cable or bluetooth or wlan or Lan. There will be no middle man like router and switch.
Its advantages are low latency faster data transfer. There is not middle man which makes it faster.
Its disadvantages are we cannot build this for more than two devices.


### *Daisy chain*

![[Pasted image 20250418235243.png]]

In this topology every device connects to other device using a wire like a device connects to b with one wire and b device connects to c using another wire. it is like bus topology but it is not. In bus topology all devices listens at the same time while in daisy chain all devices listens one after another.
Its advantage is easy to add devices.
its disadvantage is one failure stops the whole network.




