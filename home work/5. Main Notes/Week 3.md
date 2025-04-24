
2025-04-24 11:10

Topic: 

Tags: 

Name: *me_as_nobody*
## *Reference*



---
## *Transport layer*

This layer control how data gets transferred reliable (TCP) or quick (UDP). It will be in kernal.
When application layer packs data and sends to Transport layer it will one TCP header or UDP header to that packet tell that packet which protocol it should follow.

This layer has two protocols to follow.
1. *Transfer control protocol(TCP)* : This is reliable protocol to transfer data from component to other. it has three way handshake method(SYN,SYN/ACK,ACK) which ensures successful delivery of data. 
2. *User datagram protocol(UDP)* : It fast and non-reliable protocol. It doesn't care data is transferred or not.

*Connection establishment* 
A normal connection established when the client requests (sends request packet to server) the connection and server acknowledge the client request in return it allow the connection(sends acknowledgment packet to client so that connection establishes). 

*The problem*
We have a problem while establishing a connection imagine a client is sending two requests to a server (Req1 and Req2). And at that time if the server crashes and restarts the server might get confused the req1 is a new request or a repeat of req2. Because when the client sending request 1 the server crashed so req1 couldn't able to get to the server. So the client didn't receive any status from the server, the client sends one more request2. Now request 1 is in queue and server receives the request2, and it also receives the request 1 now what should client think about the req1?. Req1 is called delayed duplicates. 

We need to solve this problem with no errors and give fast performance. Now we need to craft rules which can tackle this problem efficiently and smartly.

*Solution 1*
Once a port is used by the client, it should not use that same port again. so the delayed packets cant go to the same port.
But we have a problem to this what if all ports ran out?

*Solution 2*
