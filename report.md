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



# TASK 4: WORKING OF VERSION CONTROL

## INTRODUCTION

Version Control is a system that helps us save and track changes made to files over time.  
It allows us to return to previous versions, work in teams, and manage projects easily.

Git is a widely used version control tool that helps developers handle code efficiently.

---

## BASIC CONCEPTS OF VERSION CONTROL

### Repository
A repository is a place where project files and their history are stored.  
It can be:
- Local repository (on our computer)
- Remote repository (on GitHub or GitLab)

### Commit
A commit is used to save changes made to files.  
Each commit has a unique ID and a message describing the changes.

### Branch
A branch allows us to work on new features without affecting the main code.

### Merge
Merge is used to combine changes from one branch into another.

---

## INSTALLING AND INITIALIZING GIT

To check if Git is installed:
```bash
git --version
```

## INITIALIZING A NEW REPOSITORY
```bash
git init
```


---

## GIT COMMANDS PRACTICED

### 1. `git branch`

The `git branch` command is used to **create and manage branches**.

**Create a new branch**

`git branch branch-name` 

**List all branches**

`git branch` 

**Create and switch to a branch**

`git checkout -b branch-name` 

**Switch between branches**

`git checkout branch-name` 


----------

### 2. `git merge`

The `git merge` command is used to **merge one branch into the current branch**.

**Syntax**

`git merge branch-name` 

This command combines the changes from the given branch into the active branch.


    

----------

### 3. `git revert`

The `git revert` command is used to **undo a commit safely**.

**Syntax**

`git revert commit-hash` 

It creates a new commit that reverses the changes made by a previous commit.



----------

### 4. `git cherry-pick`

The `git cherry-pick` command is used to **apply a specific commit** from another branch.

**Syntax**

`git cherry-pick commit-hash` 

This command is useful when only a particular commit is required.

📸 _Screenshots:_
![osi](https://github.com/yasmeen-taj111/images/blob/main/git1.jpeg?raw=true)

![osi](https://github.com/yasmeen-taj111/images/blob/main/git2.jpeg?raw=true)

![osi](https://github.com/yasmeen-taj111/images/blob/main/git3.jpeg?raw=true)











----------

# Task 5: DYNAMODB

## 1. INTRODUCTION

This project demonstrates a **secure user login system** implemented using **AWS DynamoDB**. The system allows users to **register** and **log in** using email and password credentials. Passwords are securely stored using **hashing**, ensuring data security.

**Technologies Used:**

-   Python 3
    
   
-   AWS DynamoDB (NoSQL Database)
    
-   Boto3 (AWS SDK for Python)
    
-   bcrypt (for password hashing)
    

----------

## 2. OBJECTIVES

-   Understand the basics of **NoSQL databases** and how DynamoDB works.
    
-   Implement a **secure registration and login system**.
    
-   Learn to interact with AWS services using **Boto3**.
    
-   Compare **SQL vs NoSQL** databases and understand their use cases.
    

----------

## 3. DYNAMODB OVERVIEW

**Amazon DynamoDB** is a fully managed **NoSQL database** service. It provides:

-   **Scalability:** Handles traffic from a few requests per second to millions without manual intervention.
    
-   **Performance:** Offers low-latency read and write operations.
    
-   **Flexible Schema:** Supports different data structures, unlike rigid SQL tables.
    
-   **Integration:** Works seamlessly with other AWS services.
    

**Key Concepts:**

-   **Table:** Collection of items (similar to SQL tables).
    
-   **Item:** Individual records in a table (like rows in SQL).
    
-   **Attributes:** Fields of an item (like columns in SQL).
    
-   **Primary Key:** Uniquely identifies each item.
    

----------

## 4. DIFFERENCE BETWEEN MYSQL AND NOSQL

| Feature        | MySQL               | NoSQL (DynamoDB)      |
|----------------|-------------------|----------------------|
| Data Structure | Rows and Columns (Tables) | Key-Value / Document  |
| Schema         | Fixed              | Flexible             |
| Query Language | SQL                | Varies / API calls   |
| Scalability    | Vertical           | Horizontal           |

----------

## 5. SYSTEM WORKFLOW

### 5.1 Registration

1.  User enters **email** and **password**.
    
2.  Password is **hashed** using bcrypt.
    
3.  User credentials are stored in DynamoDB table `signup_page`.
    

**Example Output:**

```
Enter email: yasmeen_taj
Enter password: 1234
SUCCESS: User yasmeen_taj registered with a hashed password.

```

### 5.2 Login

1.  User enters **email** and **password**.
    
2.  System retrieves the hashed password from DynamoDB.
    
3.  Password is verified against the hash.
    
4.  User is granted access if credentials match.
    

**Example Outputs:**

```
Enter email: yasmeen_taj
Enter password: 1234
WELCOME: Login successful for yasmeen_taj!

```

```
Enter email: yasmeen_taj
Enter password: 123
FAILED: Invalid email or password.

```

----------


## 6. IMPLEMENTATION DETAILS

**File Structure:**

```
user-login-system/
├── app.py              # Main program (CLI or Flask interface)
├── auth_service.py     # Handles registration and login logic
├── database.py         # DynamoDB connection setup using Boto3
├── requirements.txt    # Python dependencies
└── .env                # Environment variables (AWS keys)

```

**Python Libraries Used:**

-   `boto3` – AWS SDK to interact with DynamoDB
    
-   `bcrypt` – For secure password hashing
    
-   `python-dotenv` – Load AWS credentials from `.env` file
    

**Key Code Snippets:**

# Hashing password
hashed_password = bcrypt.hashpw(password.encode('utf-8'), bcrypt.gensalt())

# Verifying password
```
if bcrypt.checkpw(input_password.encode('utf-8'), stored_hash.encode('utf-8')):
    print("Login successful")
else:
    print("Invalid credentials") 

```

----------

## 7. TERMINAL OUTPUTS

**Login Attempts:**

-   Correct password → Login successful.
    
-   Incorrect password → Login failed.
    
-   Multiple users supported.
    

----------

## 8. LEARNING OUTCOMES

-   Learned to set up **AWS CLI** and configure credentials.
    
-   Learned to use **Boto3** for CRUD operations in DynamoDB.
    
-   Implemented **secure password storage** using bcrypt.
    
-   Understood **differences between SQL and NoSQL** databases.
    
-   Developed a **working user login system**.
    

----------

## ScreenShote

![osi](https://github.com/yasmeen-taj111/images/blob/main/db1.jpeg?raw=true)
![osi](https://github.com/yasmeen-taj111/images/blob/main/db2.jpeg?raw=true)





## GITHUB REPOSITORY

Github project repository:  
[https://github.com/yasmeen-taj111/dynamodb-user-login-system](https://github.com/yasmeen-taj111/dynamodb-user-login-system)

----------







# TASK 7: Encryption Techniques - Secure Messaging App

## 1. Introduction

Encryption protects messages by converting plaintext into ciphertext, ensuring only authorized users can read them. This project demonstrates secure messaging using **AES (Advanced Encryption Standard)** in Python, allowing messages to be encrypted before sending and decrypted upon receipt.

----------

## 2. Encryption Techniques

### AES (Symmetric Encryption)

-   Uses a **single secret key** for encryption and decryption.
    
-   Fast and secure for message transmission.
    
-   Process:
    
    1.  Sender encrypts plaintext with the secret key → ciphertext.
        
    2.  Ciphertext is transmitted over the network.
        
    3.  Receiver decrypts it using the same key → original message.
        

**Other ciphers learned:** Caesar, Vigenère, and Substitution. These are simpler but less secure.


### Symmetric vs Asymmetric Encryption

| Feature      | Symmetric (AES)        | Asymmetric (RSA)                   |
|--------------|------------------------|------------------------------------|
| Keys Used    | 1 (same key)           | 2 (public & private)               |
| Security     | Key must be shared securely | Public key can be shared openly |
| Use Case     | Messaging              | Digital signatures, key exchange   |

**RSA** relies on large prime numbers to generate secure public–private key pairs.


----------

## 3. Project Implementation

-   Python libraries: `PyCryptodome`, `base64`.
    
-   Functions:
    
    -   **Encrypt message:** Converts plaintext → ciphertext.
        
    -   **Decrypt message:** Converts ciphertext → original plaintext.
        

**Sample Run:**

```
Message: Hello World
Encrypted: yvyhyEf2469lW35wQ8+ZvyjmSsiWJ5000sWtjU/6Zsc=
Decrypted: Hello World

```

----------

## 4. Conclusion

-   AES encryption ensures secure communication over insecure networks.
    
-   RSA introduces asymmetric encryption for secure key exchange.
    
-   Classic ciphers provide foundational understanding but are not practical for modern security.
    
-   This project forms a strong base for building **secure chat applications**.
    

**GitHub:** [Encryption Chat Box](https://github.com/yasmeen-taj111/Encryption-Chat-box)

----------

![osi](https://github.com/yasmeen-taj111/images/blob/main/en1.jpeg?raw=true)
![osi](https://github.com/yasmeen-taj111/images/blob/main/en2.jpeg?raw=true)












# TASK 7: IP Addressing and Web Scraping – Job Listings Scraper

## Objective
The objective of this task was to understand **web scraping using Python** and relate it to **IP addressing and TCP/IP protocols**. Using the `requests` and `BeautifulSoup` libraries, a scraper was developed to extract structured data from a website and store it in a CSV file.

---

## Tools & Technologies Used
- **Python**
- **requests** – to send HTTP requests
- **BeautifulSoup (bs4)** – to parse HTML content
- **CSV module** – to store extracted data


---

## Implementation Overview
- A GET request is sent to the website using the `requests` library.
- The HTML response is parsed using **BeautifulSoup**.
- Book details such as **Title, Price, and Availability** are extracted.
- The top 10 records are stored in an `output.csv` file.

``` python
requests.get(url)
```

This line internally uses TCP/IP protocols to establish a connection between the client and server using IP addresses.


---

Sample Extracted Data (output.csv)


| Title                  | Price  | Availability |
|------------------------|--------|--------------|
| A Light in the Attic    | £51.77 | In stock     |
| Tipping the Velvet    | £53.74 | In stock     |
| Soumission             | £50.10 | In stock     |




---

IP Addressing & TCP/IP Relevance

Each HTTP request sent by the scraper uses the IP address of the target server.

TCP ensures reliable data transfer.

IP handles routing of data packets between client and server.

This demonstrates how web applications rely on networking fundamentals.



---

Conclusion

This task successfully demonstrated:

Practical web scraping using BeautifulSoup

Data extraction and storage in CSV format

Real-world application of IP addressing and TCP/IP protocols


The project reinforces both networking concepts and Python automation skills, forming a strong foundation for advanced scraping and data analysis tasks.


---

GitHub Repository

🔗 https://github.com/yasmeen-taj111/WebScraping


![osi](https://github.com/yasmeen-taj111/images/blob/main/sc1.jpeg?raw=true)



