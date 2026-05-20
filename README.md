# my-nginx-ssh-project
# AWS EC2 Cloud Infrastructure Deployment: Ubuntu & Nginx Web Server

A hands-on DevOps and cloud infrastructure project demonstrating how to launch an AWS EC2 instance using Ubuntu Linux, configure secure networking, install an Nginx web server, and deploy a custom webpage. 

This repository serves as documentation for configuring public cloud servers, handling Linux-based network firewalls, and managing server deployment workflows entirely over an SSH client.

---
## 🧭 Key Concepts Explained

Building this setup requires understanding how several decoupled cloud and networking layers interact to serve web content securely:

* **EC2 Instance (Elastic Compute Cloud):** A virtual computing environment in AWS. Think of it as a blank-slate computer sitting in an Amazon data center that we lease and manage remotely.
* **SSH (Secure Shell):** A cryptographic network protocol used to run a secure command-line session on our remote server over an unsecure network.
* **Security Groups (Cloud Firewall):** AWS's virtual firewalls that control inbound and outbound infrastructure traffic. By default, they block everything except SSH access to protect the server.
* **UFW (Uncomplicated Firewall):** The built-in operating system firewall for Ubuntu. It acts as an inner layer of security behind the AWS Security Group.
* **Nginx Web Server:** High-performance software designed to listen for network requests (like a browser asking for a page) and serve back static files like HTML, CSS, or media.

---

## 🏗️ Architecture Workflow

1. **Local Terminal (SSH Client)** ──🔑──> 2. **AWS Security Group (Port 22, 80 & 443)** ──> 3. **Ubuntu OS Firewall (UFW)** ──> 4. **Nginx Server Engine** ──> 5. **`index.nginx-debian.html`**

---

<img width="940" height="271" alt="image" src="https://github.com/user-attachments/assets/ff8429da-f089-42c4-a64a-de7c7931f1c3" />
