

# TASK 6: Encryption Techniques - Secure Messaging App

## 1. Introduction

Encryption protects messages by converting plaintext into ciphertext, ensuring only authorized users can read them. This project demonstrates secure messaging using **AES (Advanced Encryption Standard)** in Python, allowing messages to be encrypted before sending and decrypted upon receipt.

----------

## 2. Encryption Techniques

### AES (Symmetric Encryption)

- Uses a **single secret key** for encryption and decryption.

- Fast and secure for message transmission.

- Process:

1. Sender encrypts plaintext with the secret key → ciphertext.

2. Ciphertext is transmitted over the network.

3. Receiver decrypts it using the same key → original message.


**Other ciphers learned:** Caesar, Vigenère, and Substitution. These are simpler but less secure.


### Symmetric vs Asymmetric Encryption

| Feature | Symmetric (AES) | Asymmetric (RSA) |
|--------------|------------------------|------------------------------------|
| Keys Used | 1 (same key) | 2 (public & private) |
| Security | Key must be shared securely | Public key can be shared openly |
| Use Case | Messaging | Digital signatures, key exchange |

**RSA** relies on large prime numbers to generate secure public–private key pairs.


----------

## 3. Project Implementation

- Python libraries: `PyCryptodome`, `base64`.

- Functions:

- **Encrypt message:** Converts plaintext → ciphertext.

- **Decrypt message:** Converts ciphertext → original plaintext.


**Sample Run:**

```
Message: Hello World
Encrypted: yvyhyEf2469lW35wQ8+ZvyjmSsiWJ5000sWtjU/6Zsc=
Decrypted: Hello World

```

----------

## 4. Conclusion

- AES encryption ensures secure communication over insecure networks.

- RSA introduces asymmetric encryption for secure key exchange.

- Classic ciphers provide foundational understanding but are not practical for modern security.

- This project forms a strong base for building **secure chat applications**.


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


| Title | Price | Availability |
|------------------------|--------|--------------|
| A Light in the Attic | £51.77 | In stock |
| Tipping the Velvet | £53.74 | In stock |
| Soumission | £50.10 | In stock |




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


---



# **Task 8: Creating and Deploying an Application on EC2**

## **Objective**

To launch and configure an EC2 instance on AWS and deploy a dynamic backend application.

## **Implementation Summary**

An EC2 instance was created using Ubuntu 22.04 LTS with a `t3.micro` instance type. Security Groups were configured to allow SSH (22) and application traffic (8000).

The FastAPI backend of the **Geo Rep Lookup** project was cloned from GitHub and deployed on the instance. A Python virtual environment was created, dependencies were installed using `requirements.txt`, and the application was run using Uvicorn.

## **Outcome**

The backend API was successfully deployed and accessed publicly via the EC2 public IP address. This task provided practical experience in EC2 instance management, server configuration, and deploying a dynamic backend application in the cloud.


![fastapi](https://github.com/yasmeen-taj111/images/blob/main/terminal.jpeg?raw=true)
![terminal](https://github.com/yasmeen-taj111/images/blob/main/WhatsApp%20Image%202026-02-27%20at%2007.25.55.jpeg?raw=true)
---

# **TASK 9: AWS CloudFront - Serve content from multiple S3 buckets**

## **Objective**

To configure Amazon CloudFront to securely serve content from multiple Amazon S3 buckets using path-based routing and Origin Access Control (OAC).

---

## **Services Used**

* Amazon S3
* Amazon CloudFront
* Origin Access Control (OAC)

---

## **Architecture**

User → CloudFront →
• S3 Bucket 1 (HTML, CSS, JS)
• S3 Bucket 2 (Images)

CloudFront routes traffic based on path patterns:

* Default (*) → Main website bucket
* `images/*` → Images bucket

---

## **Implementation Summary**

1. Created two S3 buckets:

* Static website bucket (HTML, CSS, JS)
* Images bucket (media files)

2. Created a CloudFront distribution with both buckets as origins.

3. Configured behavior:

* Default behavior → Main bucket
* `images/*` behavior → Images bucket

4. Enabled **Origin Access Control (OAC)** to securely allow CloudFront to access private S3 buckets.

5. Added bucket policies allowing access only from the specific CloudFront distribution.

---

## **Issue Faced**

Images returned **AccessDenied** error.

### Cause:

Images bucket origin was set to Public instead of OAC.

### Resolution:

Attached Origin Access Control to the images origin and updated bucket policy. After deployment, all assets loaded successfully.

---

## **Result**

The website successfully:

* Loads HTML, CSS, and JS from Bucket 1
* Loads images from Bucket 2
* Restricts direct public access to S3
* Delivers content securely via CloudFront

---

## **Conclusion**

This project demonstrates secure multi-origin configuration using Amazon CloudFront and Amazon S3 with path-based routing and Origin Access Control, following best practices for scalable and secure static website hosting.

![s3 bucket](https://github.com/yasmeen-taj111/images/blob/main/s3%20aws.jpeg?raw=true)
![static](https://github.com/yasmeen-taj111/images/blob/main/static%20s3.jpeg?raw=true)


---






