# TASK 1: OSI MODEL


The **Open Systems Interconnection (OSI)** model is a conceptual framework that defines how computers communicate over a network.  
It divides the entire communication process into **seven layers**, each responsible for specific tasks.

This model helped me understand how different devices across the world can talk to each other smoothly through the internet — just like a teamwork of seven members, where each one has a unique role!

## THE SEVEN LAYERS OF THE OSI MODEL

### 1. Application Layer
- The topmost layer where users directly interact with applications like browsers and email clients.  
- Provides services such as email (SMTP), file transfer (FTP), and web browsing (HTTP).  
- **Common Protocols:** HTTP, FTP, SMTP, DNS, SSH, SNMP, DHCP  
- **Relation to Cloud:** Applications like Google Drive, Gmail, and AWS console work at this layer to let users access cloud services.

### 2. Presentation Layer
- Responsible for **data formatting, encryption, and compression**.  
- Ensures that the data sent by the sender is readable and usable by the receiver.  
- **Example:** Converting data into readable formats like JPEG, MP4, or text.  
- **Relation to Cloud:** Ensures data security and proper format conversion during cloud file uploads or downloads.


### 3. Session Layer
- Manages **sessions or connections** between computers.  
- Handles **establishing, maintaining, and terminating** connections.  
- Provides **authentication and synchronization** between devices.  
- **Relation to Cloud:** Manages user sessions when logging into cloud platforms like AWS, Google Cloud, or any SaaS-based applications.

### 4. Transport Layer
- Ensures **reliable and accurate data delivery** between applications.  
- Performs **segmentation, error checking, and flow control**.  
- **Protocols:**
  - **TCP (Transmission Control Protocol):** Reliable and connection-oriented.  
  - **UDP (User Datagram Protocol):** Fast but connectionless.  
- **Relation to Cloud:** Ensures reliable communication between cloud servers and clients, especially for real-time services like video streaming or online meetings.


### 5. Network Layer
- Responsible for **routing data packets** between networks.  
- Uses **logical addressing (IP addresses)** to identify devices.  
- **Protocols:** IP, ICMP, IGMP  
- Handles **path determination and packet forwarding** using routers.  
- **Relation to Cloud:** Helps in transferring data between different cloud data centers and networks efficiently.

### 6. Data Link Layer
- Ensures **error-free data transfer** between two directly connected nodes.  
- Uses **MAC addresses** for identifying devices on the same network.  
- Handles **framing, error detection, and flow control**.  
- **Relation to Cloud:** Provides a stable and secure base for virtual machines and cloud servers to communicate through data frames.



### 7. Physical Layer
- Deals with the **actual physical connection** — cables, switches, routers, and hardware components.  
- Converts data into **electrical, radio, or light signals** for transmission.  
- **Relation to Cloud:** Cloud infrastructure depends on **high-speed physical connections (like fiber optics)** for global data transfer.



Each layer is stacked vertically to represent how data moves up and down between layers — from user applications down to hardware and back up again on the receiving side.


### KEY CONCEPTS LEARNED
- **Switching:** Process of moving data packets between devices on the same network.  
- **Routing:** Deciding the best path for data to travel across different networks.  
- **Handshake:** Initial connection setup between two systems (e.g., TCP 3-way handshake).  
- **IP Addressing:** Unique logical addresses that identify devices in a network (like 192.168.x.x).



![osi](https://github.com/yasmeen-taj111/images/blob/main/OSI.jpeg?raw=true)


---



# TASK 2: IaaS, PaaS, and SaaS


Cloud computing has completely changed the way we use technology today. Instead of buying and maintaining expensive hardware and software, companies (and even individuals) can now use cloud-based services according to their needs.  

There are mainly **three types of cloud computing service models** — **IaaS, PaaS, and SaaS**.  
Each one offers a different level of control, flexibility, and management — just like building a house:  
- **IaaS** gives you the land and materials.  
- **PaaS** gives you a ready-made foundation to build on.  
- **SaaS** gives you the fully built house — ready to move in!






###  1.INFRASTRUCTURE AS A SERVICE (IaaS)
**IaaS** provides the basic building blocks for cloud IT — such as virtual servers, storage, and networking.  
It allows users to rent IT infrastructure on a pay-as-you-go basis.

### Features
- Full control over operating systems and applications  
- Highly scalable and flexible  
- Eliminates the need to buy physical hardware  

###  Example
- **Amazon Web Services (AWS EC2)**  
- **Microsoft Azure Virtual Machines**  
- **Google Compute Engine (GCE)**  

###  Relation to Cloud Computing
IaaS forms the **foundation layer** of cloud computing. Developers or businesses use it to create virtual data centers that can host websites, apps, or even entire enterprise systems.


### 2. PLATFORM AS A SERVICE (PaaS)
**PaaS** provides a platform that lets developers build, test, and deploy applications without worrying about managing the underlying infrastructure.

### Features
- Offers a pre-configured environment for coding and deployment  
- Includes operating systems, databases, and development tools  
- Reduces time needed to develop and launch apps  

###  Example
- **Google App Engine**  
- **AWS Elastic Beanstalk**  
- **Microsoft Azure App Service**  

### Relation to Cloud Computing
PaaS helps developers **focus on writing code** rather than maintaining servers. It’s ideal for teams building scalable applications quickly, such as web apps or mobile apps.

### 3.SOFTWARE AS A SERVICE (SaaS)
**SaaS** delivers fully functional applications over the internet. Users can access them via a browser without installing anything locally.

###  Features
- No installation or maintenance required  
- Accessible anytime, anywhere  
- Automatic updates and data backups  

###  Example
- **Google Workspace (Docs, Gmail, Drive)**  
- **Microsoft 365**  
- **Salesforce**, **Zoom**, **Canva**  

###  Relation to Cloud Computing
SaaS is the **topmost layer** of cloud computing that most end-users interact with daily. It’s ideal for businesses and individuals who just want to use the service — without dealing with the backend.



##  COMPARISON TABLE

| Feature | IaaS | PaaS | SaaS |
|----------|------|------|------|
| **User Control** | High | Medium | Low |
| **User Type** | System Admins | Developers | End Users |
| **Example** | AWS EC2, Azure VM | Google App Engine, AWS Beanstalk | Gmail, Canva, Zoom |
| **Management** | User manages OS, apps, runtime | User manages apps only | Everything managed by provider |
| **Use Case** | Hosting websites, storage | App development | Communication, collaboration |


Through this task, I understood that **IaaS, PaaS, and SaaS** are like different levels of service in the cloud — from renting raw infrastructure to using ready-made applications.  

Each model fits specific needs:  
- **IaaS** for flexibility and control,  
- **PaaS** for easy app development,  
- **SaaS** for instant software access.  

Together, they make cloud computing efficient, scalable, and accessible to everyone — from startups to global enterprises.
![osi](https://github.com/yasmeen-taj111/images/blob/main/Cloud-Service-Models-Saas-IaaS-Paas-%E2%80%93-Choose-the-Right-One-for-Your-Business.jpg.webp?raw=true)

---

# TASK 3: Socket IO

**Socket.IO** is a JavaScript library that enables real-time, bi-directional communication between web clients and servers.  
It works on top of the WebSocket protocol and provides additional features like fallback options, automatic reconnection, and event-based communication.

This means when one user sends a message, others connected to the same server can instantly receive it — making it perfect for applications like chat systems, live updates, or multiplayer games.


I created a **basic chat application** using **Node.js** and **Socket.IO**. The application allows multiple users to connect to the same chatroom and exchange messages in real-time.

**GitHub Repository:** [socketio-chatApp](https://github.com/yasmeen-taj111/socketio-chatApp)
![osi](https://github.com/yasmeen-taj111/images/blob/main/socketio.jpeg?raw=true)

---
