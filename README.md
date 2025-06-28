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

OSPF - Open Shortest Path First. It finds the shortest path for data to travel. It is used mainly within large organisations. It uses **Link State Information** to make routing decisions, which means it considers the status of a network, links and costs to use them. It can quickly recalculate routes when there are changes in the network.

BGP - Border Gateway Protocol. It is used to route data between different autonomous systems. BGP uses a **PAth Vector Mechanism**. This means it maintains the path formation that gets updated dynamically as the network topology changes. BGP allows network admins to define routing policies based on various attributes, this provides greater control on how traffic flows through the network. 

----------------------------------------------------------------------------------------------------------------------------
**Subnetting & CIDR**

![image](https://github.com/user-attachments/assets/70625e40-a8c2-4e14-94cf-022c63238f45)

CIDR - Classless Inter Domain Routing. A method for allocating IP addresses and routing IP packets.

----------------------------------------------------------------------------------------------------------------------------
**Binary: Yep 1s and 0s**

![image](https://github.com/user-attachments/assets/2d8af2cc-06be-4303-ab56-eb73e7b64d62)

![image](https://github.com/user-attachments/assets/99cf1f51-89e7-4b16-bb00-3704e893817b)

----------------------------------------------------------------------------------------------------------------------------
**Calculating Subnets**

Subnetting is process of dividing a large network into smaller subnetworks, known as Subnets. This process helps to organise and manage IP addresses much more efficiently. Subnetting determines which part on the IP address is the network portion and which part is the host portion. 

Subnet Mask - Used to divide an IP address into a network and host portions. It helps routers determine which part of an IP address is the network address, and which part is the host address. 

![image](https://github.com/user-attachments/assets/217293e5-5b0a-4a7b-aab3-f8bf132b7648)

----------------------------------------------------------------------------------------------------------------------------
**NAT (Network Address Translation)**

NAT translates private IP addresses into public address. 

**Types of NATs**

Static NAT: Maps a single private IP address to a single public IP address (like having a dedicated translator for just one device). Static NAT is one-to-one mapping for fixed IP nneds.

Dynamic NAT: Maps a private IP address to one of many public IP addresses from a pool. 

PAT (Port Address Translation): Known as NAT overload. PAT is very efficient because it allows multiple devices on a local network to be mapped to a single public IP address but with different port numbers. PAT uses a single public IP from multiple devices by assigning different port numbers. 

**Troubleshoot with ping, traceroute, nslookup!**

`ping` - It is a command to test any connectivity between devices. E.g ping google.com.

`traceroute` - This command tracks the path of the data to reach its certain destination.  E.g. traceroute google.com. 

`nslookup` - Another basic tool for querying DNS to find an IP address associated with domain name. E.g. nslookup google.com.

*Practical Example: "I can't reach a website, how can I troubleshoot?"* 

1. Check network connectivity - ensure machine has working netwrok connection. Use ping command. Then, do a dig or nslookup command to verify there is no issue with the DNS. 

2. Check host file - ensure there is no overiding entries.

3. Check Firewall rules - enbsure a firewall is not blocking any outgoing/incoming traffic.

4. Check browser issues - Ensure to close the browser and start it again.

5. Check DNS cache - It may need to be cleared

6. Check system logs - do the traceroute command to check for netowrk hops.

----------------------------------------------------------------------------------------------------------------------------
**Cloud Networking!**

Cloud networking is the practice of managing and configuring networks in cloud environments. 

Very important in devops - Ensures that our applications and services can communicate efficiently and securely.

*Key components*

• VPCs (Virtual Provate Clouds) - It is a private network in the cloud. It can define the IP address range, create subnets and configure route tables and gateways. It is like a data centre but in the cloud. 

• Subnets - Help to organise a network and control the flow of traffic. You can have different subnets for different types of resources e.g. one for application server, one for databases etc. 

• Gateways - What connects the VPC to the outside world e.g. the internet. They handle incoming/outgoing traffic and ensure the resources can communicate with external networks 

----------------------------------------------------------------------------------------------------------------------------
# NGINX EC2 Deployment

This project documents the deployment of an NGINX web server on an AWS EC2 instance and exposes it via a custom domain through 
Cloudflare DNS.

## 🌩️ EC2 (Elastic Compute Cloud)

Amazon EC2 is a service provided by AWS (Amazon Web Services) that lets you rent virtual servers (called instances) in the 
cloud. These servers can run applications, websites, or anything you'd run on a physical server — but without needing to 
buy hardware.

---

## 🌐 Cloudflare

Cloudflare is a service that sits between your website and visitors, providing:

• DNS management (mapping domain names to IPs)

• DDoS protection (blocks bad traffic)

• Content delivery (CDN) (speeds up your site)

• SSL/HTTPS (encrypts traffic)

---

## 🌍 DNS (Domain Name System)

DNS is like the phone book of the internet — it translates domain names (like nginx.mwaqar.co.uk) into 
IP addresses (like 13.49.212.87) so browsers can find the right server.

---

## 🕸 NGINX

NGINX is a web server software that:

• Delivers web pages to visitors

• Can act as a reverse proxy, load balancer, or API gateway

• Is known for being lightweight and fast



## 🚀 Deployment Steps

### 1️⃣ Launch EC2 Instance
- AMI: Amazon Linux 2023
- Instance type: `t2.micro`
- Security Group:
  - Allow SSH (22) — your IP only
  - Allow HTTP (80) — `0.0.0.0/0`
- Elastic IP assigned: ✅

---

### 2️⃣ Install NGINX

SSH into the EC2 instance:

ssh -i your-key.pem ec2-user@<enter IP address here>

Installed and start NGINX on the termiinal: 

`sudo dnf update -y`

`sudo dnf install nginx -y`

`sudo systemctl enable nginx`

`sudo systemctl start nginx`

Tested this:

http://<Enter IP address here>

---

### 3️⃣ Set Up Cloudflare DNS

Added A record:

Type: A

Name: nginx

Content: <enter IP address here>

Proxy status: DNS Only (gray cloud)

Tested this:

http://nginx.mwaqar.co.uk

---

### 🌐 Domain & DNS

Domain: mwaqar.co.uk

Subdomain: nginx.mwaqar.co.uk

Managed via Cloudflare

![image](https://github.com/user-attachments/assets/96546d96-19d9-4e57-b8a0-0316a8fb2eba)
