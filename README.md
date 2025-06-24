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

*Transmission Control Protocol (TCP)* is the postman of the internet. It ensures data sent from one device reaches another device accurately and in the correct order. It's a protocol, which means that it's a set of rules that devies follow to communicate with each other. "Handshake" - to confirm that you are on the same page. TCP ensures data is delivered in order. TCP checks for errors and controls the flow of data to prevent congestion, ensuring smooth and error free communication. TCP is used whenever two devices need to exchange data back and forth e.g. web browsing, emails & file transfers. 

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

--------------------------------------------------------------------------------------------------------------------------- 
**OSI layers: POV of Sender & Receiver**

![image](https://github.com/user-attachments/assets/e7663b7e-c0f4-47c1-bd9f-aea54e47f983)

![image](https://github.com/user-attachments/assets/1506fdb0-d33d-40cd-984a-e449a6ebf493)

-----------------------------------------------------------------------------------------------------------------------------
**What is DNS (Domain Name System)**

DNS allows humans to keep track of websites and hosts by name instead of an IP address. Bit like a contact list where you know somenone by name but cannot remember their phone number. DNS translates domain name into IP addresses. In networking, DNS simplifies navigation on the internet. It is essential for accessing websites and services. 

----------------------------------------------------------------------------------------------------------------------------
**DNS Components: Nameservers & Zone Files.**

*Name Servers* - • Load DNS setting and configurations. • Can be authoritative or recursive. 

*Zone Files* - •Store information about the domain. • Organised and readable format. 

----------------------------------------------------------------------------------------------------------------------------
**DNS Records**

![image](https://github.com/user-attachments/assets/cc166dc7-b3bc-4ef9-9cb6-e3695306903e)

-----------------------------------------------------------------------------------------------------------------------------
**DNS Hierarchy & Distribution**

![image](https://github.com/user-attachments/assets/af89ecd7-a58a-4366-bb59-f44926050920)

-----------------------------------------------------------------------------------------------------------------------------
**DNS Resolution Process**

![image](https://github.com/user-attachments/assets/098613da-f692-409a-b6e9-f6e39e7166f5)

-----------------------------------------------------------------------------------------------------------------------------
**How Does DNS Work??**

![image](https://github.com/user-attachments/assets/d4a8f561-5d16-49b4-bd82-7f9ce3a2df86)

-----------------------------------------------------------------------------------------------------------------------------
**Understanding the /etc/hosts file**

*What is /etc/hosts?* 

- It is a local file on the computer. It maps the domain name to the IP addresses. It takes precedence over DNS for specific entries.  

-----------------------------------------------------------------------------------------------------------------------------
**Routing**

![image](https://github.com/user-attachments/assets/97f674b8-6e91-473e-a42b-00661f0aea3c)

![image](https://github.com/user-attachments/assets/158cd49f-dc22-46fe-b388-51b2faec2524)

![image](https://github.com/user-attachments/assets/8954d952-ca55-467b-95c3-9713edcafa6f)

----------------------------------------------------------------------------------------------------------------------------
**Static vs. Dynamic Routing**

Static routing involves manually configuring routes in the network. These routes are **fixed** and do not change unless mainly updated by **network admin**. Static routing is simple to set up but it is not scalable. It is great for small and stable networks for small companies. 

Dynamic routing automatically adjusts routes based on current network conditions. It's like having a smart GPS that updates the route if there is traffic or roadblock. Dynamic routing relies on route protocols to find the best path for data. These protocols help routers communicate and decide on the most efficient route. Benefit of dynamic routing compared to static is that it is scalable and adaptable, making it suitable for large and complex networks. It responds to changes in the network, e.g. new devices or failed connections without manual intervention. Dynamic routing protocols **automatically** update routes to optimise the traffice flow and handle network changes seamlessly. 

----------------------------------------------------------------------------------------------------------------------------
**Common Routing Protocols**

The use algorithms to figure out the best paths for data to travel from one place to another. Routing protocols are important because they automate route updates and improve network resilience by finding alternative paths.

#OSPF and BGP



