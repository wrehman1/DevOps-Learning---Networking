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


