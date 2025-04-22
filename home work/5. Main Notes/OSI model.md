
2025-04-19 12:00

Topic: 

Tags: 

Name: *me_as_nobody*
## *Reference*



---

## *What is the OSI model ?*

The Open systems interconnection (OSI) model is a framework how systems communicate with each other. It is created by ISO (International Standardization of Organization).
Its is like blueprint how networking devices communicate with each other.

*The OSI model has 7 layers*
### *1. Physical layer*

The physical layer handles the physical connections between devices like it handles how cable are connected and it will send data through wires. This layers turns binary data into electrical, optical and radio signals that travel over cables, fibers or WIFI and vice versa.

This layer covers cables (coaxial, twisted pair), connectors (RJ45, SC) and signaling methods (voltage for ethernet and light for fibers).

### *2. Data link layer*

The data link layer takes bits from layer 1 (physical layer) and packages them into frames for reliable data transfer between two directly connected devices.
It adds header and trailer. Protocols and WIFI work here with their standards.

### *3. Network layer*

The network layer manages routing of packets across a different network. it uses protocols like Internet protocol to identify devices.

### *4. Transport layer*

This layer ensures delivery. It manages end to end communication of device, error checking and data segmentation. it is like traffic manager of your data.
TCP ensures three level handshake and acknowledgments. UDP is faster but not reliable. It is used in streaming.

### *5. Session layer*

The Session layer manages and controls the sessions between applications, handling starts, maintenance, and end of session.
It provides checkpoint and recovery if connection stops.
Protocols like NETBIOS operates here.

### *6. Presentation layer*

The presentation layer translates data to a format app can use. Handling encryption, compression and conversion. it manages SSL/TLS for secure websites. Its a translator for network and user.


### *7. Application layer*

The application layer supports the software that users interact with - browsers, Gmail, games.
Its the interface between you and the network.
Protocols like HTTP/HTTPS, DNS live here.

