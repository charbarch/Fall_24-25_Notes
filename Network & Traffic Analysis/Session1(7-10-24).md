
# Network Protocols and Packet Analysis

## Most Famous Network Protocols
- **TCP (Transmission Control Protocol)** and **UDP (User Datagram Protocol)** are the two most famous network protocols.

## Packet Analysis
- When analyzing network traffic, you typically examine the **source MAC address**, **IP address**, **protocol**, and **port number**.

## TCP and UDP:
- **TCP** (Transmission Control Protocol) is a connection-oriented protocol. It ensures reliable data delivery by **acknowledging packets and resending lost ones**.
- **UDP** (User Datagram Protocol) is connectionless and **does not guarantee delivery** or **retransmit lost packets**. It is faster but less reliable than TCP.

## Understanding Application Layer Protocols
- It's important to understand how applications like **HTTP, HTTPS, and SSH** work, how they send and receive data over the network.

## SSH (Secure Shell)
- **SSH** is an application layer protocol used to securely transfer data between two parties. It typically operates over **TCP**, not UDP.
  
## Data Transfer via TCP and UDP
- **TCP** and **UDP** are responsible for transferring data. They act like "trains" that carry data for higher-level protocols such as **HTTP**, **HTTPS**, and **SSH**.
  
## Network Data Transfer
- A network takes all your data and carries it to its destination, using **TCP**, **UDP**, or other protocols like **DHCP**.

## Software and Protocols
- Application layer protocols include **HTTP, HTTPS, SSH**, and **FTP**.
  
## Data Transmission Example
- When you make a request to a website like `http://www.aust.edu.lb`, you're using **HTTPS**. The request is converted to an **IP address**, and the data is sent to a specific port (e.g., **port 443** for HTTPS). The combination of IP address and port is known as a **socket**.

## Protocols and Ports
- Every protocol listens on a specific port. For example:
  - **HTTP**: Port **80**
  - **HTTPS**: Port **443**
  - **SSH**: Port **22**
  - **DNS**: Port **53**
  - **FTP**: Ports **20/21**
  
- Servers have processes that listen on these ports. For example:
  - **HTTP** is handled by the **httpd** server process.
  - **SSH** is handled by the **sshd** process.
  - **FTP** is handled by the **ftpd** process.

## Main Servers
- **SMTP** (Simple Mail Transfer Protocol) is used for sending email, and it typically runs on **port 25**.

## Client-Server Interaction
- **HTTP** is a protocol used by clients (like web browsers) to make requests to servers. The client sends requests, and the server responds.

## Hackers and Network Traffic
- When a hacker sends a malicious packet, it still goes through **TCP or UDP**.
- **Legitimate** and **illegitimate** packets can be identified by analyzing the traffic.
- For example, you can detect an **SQL injection** attack and block it at the **network layer** using tools like **Wireshark**.

## Network Packet Analysis
- **Wireshark** is a tool used for analyzing packets in real-time, helping detect both normal and malicious traffic.
