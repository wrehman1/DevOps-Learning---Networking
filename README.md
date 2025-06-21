# DevOps-Learning---Networking
-----------------------------------------------------------------------------------------------------------
**Overview of Computer Networks**

Definition: Connecting devices to share information.

Purpose: Communication & resource sharing. 

*Core types of Networks:* 

  • LAN - Local Area Network (Home network. Small & covers a limited area)
  
  • WAN - Wide Area Network (Wider range. Institutions and businesses etc)

*Importance in modern infrastructure*

![image](https://github.com/user-attachments/assets/050a1a11-9e61-4ff6-96a6-74e991706322)

*Networking in Devops* 

![image](https://github.com/user-attachments/assets/373eafc6-5e07-4215-8745-7627576010eb)

-----------------------------------------------------------------------------------------------------------
**LAN & WAN**

![image](https://github.com/user-attachments/assets/58be542d-317d-4312-bdfc-daae9d3bb6c7)

----------------------------------------------------------------------------------------------------------
**Switches, Routers and Firewalls**

![image](https://github.com/user-attachments/assets/e523a984-73dc-4846-90ba-9f040a139929)

------------------------------------------------------------------------------------------------------------ 
**IP address & MAC address**

![image](https://github.com/user-attachments/assets/60f5a1e3-b491-49f2-9d3a-1bcac98d719f)

![image](https://github.com/user-attachments/assets/81ac5f43-ce00-4acf-80f4-01fefb0bca19)

-------------------------------------------------------------------------------------------------------------
**Ports & Protocols: TCP, UDP**

Ports are logical doors on the device. Each door is numbered and each number for a specific type of network communication. Web traffice goes through port 80 (HTTP) and port 443 (HTTPS). These ports help facilitate communications betweeen devices. When the computer wants to send data or receive data, it uses these ports to make sure data goes to the right place. 

Protocols are rules governing data transmission. They define how data is formatted and transmitted across a network. Protocols ensure that devices can communicate effectively by following the same set of rules.

*Transmission Control Protocol (TCP)* is the postman of the internet. It ensures data sent from one device reaches another device accurately and in the correct order. It's a protocol, which means that it's a set of rules that devies follow to communicate with each other. "Hannshake" - to confirm that you are on the same page. TCP ensures data is delivered in order. TCP checks for errors and controls the flow of data to prevent congestion, ensuring smooth and error free communication. TCP is used whenever two devices need to exchange data back and forth e.g. web browsing, emails & file transfers. 

*User Diagram Protocol (UDP*) is connectionless. It is a simple protocol to send and receive data. No Prior conmmunication needed. Data can be sent immediately without waiting to establish a conenction, downside is that there is no guarantee that data will reach its destination. UDP is faster than TCP however speed comes at a cost of reliability. Suitable for real-time apps like video streaming, online gaming etc. 

![image](https://github.com/user-attachments/assets/b95dbba1-798d-45bf-bac6-7006a14639d5)

---------------------------------------------------------------------------------------------------------------------------
**The 7-layers of the OSI Model**

A communication model provides a standard framework that simplief the way devices and applications communicate over a network. 

![image](https://github.com/user-attachments/assets/57c776bb-5fc4-4fed-9224-5227256c169a)

Layer 1: Physical Layer transmits raw bit streams over a physical medium. (Cables, switches etc).

Layer 2: Provides node to node data transfer and detects and possibly corrects errors that may occue in physical layer. It ensures data is transferred correctly between adjacent network nodes. (MAC addresses, switches & bridges).

Layer 3: Determine how data is sent to the recipient. Manages packet forwarding inc routing through intermediate routers.

Layer 4: Responsible for providing reliable data transfer services to the upper layers.

Layer 5: Responsible for three things, establishing, managing and terminating sessions.

Layer 6: Translates data between the applications layer and the network. Ensures that data is in a usable format. (Encryption, data formatting).

Layer 7: Provides network services directly to the applications. 

---------------------------------------------------------------------------------------------------------------------------
**TCP/IP Model: A Commonly Used Model**

![image](https://github.com/user-attachments/assets/34ed54fa-24a8-4dbc-94ef-97eadb235359)





