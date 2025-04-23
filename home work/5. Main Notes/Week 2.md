
2025-04-23 10:32

Topic: 

Tags: 

Name: *me_as_nobody*
## *Reference*



---

## *Application layer*

The spot where users and services talk to each other. 

*Application layer  protocols examples*
1. Domain Name system.
2. File transfer protocol.
3. Hypertext transfer protocol.
4. Simple mail transfer protocol.
5. Simple network management protocol.
6. Telnet.

### *what is Domain name system?*

If we want to access a website we need to enter its IP, which is very hard to remember solution for this is domain name system, we can just type plain text to a particular website. It is much easier to use and memorize.

*There are some top level domains*

![[Pasted image 20250423105158.png]]

there are sub-domains also like 
![[Pasted image 20250423105704.png]]

#### *Fully qualified domain names*

If a domain name is ends with dot, it is assumed to complete and it is called fully qualified domain name. If a domain name doesn't end with dot it is said to be incomplete, resolver may complete this by appending a suffix to domain name.

Top level names are called the top level domains and can be three character or more in length.
These are registered and maintained by the internet corporation for assigned names and numbers (ICANN) 

Some TLD's are....
![[Pasted image 20250423111345.png]]

A zone covers domain and its subdomain defined by a start of authority. Basically domains are divided into zones which are responsible for which individual servers are responsible.
Each domain name is typically served by two DNS servers redundancy.

- Primary server contains master copy of the data for the zone.
- Secondary server gets copies of this data through zone transfer.

*zone transfer*

- Primary server loads all the data from the disk file.
- Secondary server loads all the data from the primary server. when this happens it is called zone transfer.

*Types of domains.*

*Inverse domain* : it is used to map an IP address to domain name. and it is used to prevent spam by checking a spam with a IP address has a valid domain name.

*Generic domains* : These are top level domains they aren't tied to any specific country or region. Unlike TLD's like .uk, .in they are broad, general purpose TLD's managed by ICANN (internet corporation for assigned names and numbers).

*Country domains* : These are two lettered top level domains which are linked specific countries.

### *Name resolution process*

The process how domain name turn into IP address so our device can connect to server.
*Steps*
1. Local cache check.
2. Query recursive DNS server.
3. Root server query.
4. TLD server query.
5. Authoritative server query.
6. Return and cache.

This all process is handled by BIND server. it is a open source software.

DNS database consists of Resource Records (RR). and these are divided into classes for different kinds of network. 


## *Client server model*

There are two types of servers
1. Iterative server.
2. Concurrent server.

*Iterative server*
A single copy of server runs at all times. A client may have to wait if the server is busy. It is used when server process knows how long it takes to complete one request.

*Concurrent server*
It is used when the amount of work required to handle a request is unknown, the server starts another process to handle each request. it handles multiple client connections simultaneously. 

## *TCP/UDP*

Before start of communication, a connection needs to be established between host and client.
There are five components in a connection.
1. Protocols.
2. Source IP address.
3. Source port number.
4. Destination IP address.
5. Destination port number.

*Socket*
it is used to achieve inter-process communication.
it is also combination of protocol, port number and IP.


**FTP**
it often works with TCP protocol and TELNET protocol. defined as RFC959(it defines basic mechanism of ftp). 

there are two connections
- control connection.
- data connection.
control connection receives the data on port 21.
data connection send data on port 20.