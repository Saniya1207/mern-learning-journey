# Day 02 - Internet, Browsers & DNS

## Learning Objectives

By the end of this note, you will understand:

* What the Internet is
* How websites work
* What a Browser does
* What a Server is
* What DNS is and why it is needed
* What happens when you enter a URL
* Difference between HTTP and HTTPS
* Client-Server Architecture
* Common Interview Questions

---

# 1. What is the Internet?

The Internet is a global network of computers and devices connected together that can communicate with each other.

It allows devices around the world to exchange information using standardized communication protocols.

### Examples of Devices Connected to the Internet

* Computers
* Smartphones
* Servers
* Smart TVs
* IoT Devices

### Real-Life Example

When you open:

```text
https://www.google.com
```

Your computer sends a request through the Internet to Google's server.

Google's server sends back:

* HTML
* CSS
* JavaScript
* Images

Your browser then displays the webpage.

---

# 2. What is a Browser?

A Browser is software used to access and display websites.

### Popular Browsers

* Google Chrome
* Mozilla Firefox
* Microsoft Edge
* Safari
* Brave

### Responsibilities of a Browser

A browser:

* Sends requests to servers
* Receives responses
* Renders web pages
* Executes JavaScript
* Stores cookies and cache
* Handles user interactions

### Example

When you enter:

```text
youtube.com
```

The browser:

1. Sends a request to YouTube's server
2. Receives webpage files
3. Displays the website on your screen

---

# 3. What is a Server?

A Server is a computer that stores data and provides services to clients.

A server listens for requests and sends responses.

### Examples of Servers

* Google Server
* Facebook Server
* Netflix Server
* Amazon Server

### Request-Response Cycle

```text
Client  ---- Request ----> Server

Client  <--- Response ---- Server
```

### Example

```text
Chrome Browser
        |
        v
Google Server
```

The browser requests data and the server responds with it.

---

# 4. What is DNS?

DNS stands for:

**Domain Name System**

DNS converts human-readable domain names into IP addresses.

### Why Do We Need DNS?

Humans remember:

```text
google.com
```

Computers understand:

```text
142.250.195.78
```

DNS acts as a translator between domain names and IP addresses.

---

## DNS Example

You type:

```text
www.google.com
```

DNS converts it into:

```text
142.xxx.xxx.xxx
```

Now the browser knows where Google's server is located.

---

## DNS Analogy

Think of DNS like your phone contacts.

You save:

```text
Mom
```

Instead of remembering:

```text
+91xxxxxxxxxx
```

Similarly:

```text
google.com
```

is easier to remember than:

```text
142.xxx.xxx.xxx
```

---

# 5. What is an IP Address?

IP stands for:

**Internet Protocol**

Every device connected to the Internet has a unique IP address.

### Example

```text
192.168.1.1
```

An IP address helps identify devices and allows communication between them.

---

## Types of IP Addresses

### IPv4

Example:

```text
192.168.1.1
```

* 32-bit address
* Most commonly used

### IPv6

Example:

```text
2405:201:3000::1
```

* 128-bit address
* Introduced because IPv4 addresses are limited

---

# 6. What Happens When You Visit a Website?

Suppose you enter:

```text
https://github.com
```

### Step 1

Browser reads the URL.

### Step 2

DNS lookup occurs.

```text
github.com
      |
      v
140.82.xxx.xxx
```

### Step 3

Browser finds GitHub's server.

### Step 4

A request is sent to the server.

### Step 5

Server processes the request.

### Step 6

Server sends a response.

### Step 7

Browser renders the webpage.

### Complete Flow

```text
User
 |
 v
Browser
 |
 v
DNS
 |
 v
IP Address
 |
 v
Server
 |
 v
Response
 |
 v
Browser
 |
 v
Website Displayed
```

---

# 7. What is HTTP?

HTTP stands for:

**HyperText Transfer Protocol**

It is the communication protocol used between a client and a server.

### Example

Browser Request:

```http
GET /products
```

Server Response:

```http
200 OK
```

---

## Common HTTP Methods

### GET

Used to retrieve data.

```http
GET /users
```

### POST

Used to create data.

```http
POST /users
```

### PUT

Used to update existing data.

```http
PUT /users/1
```

### DELETE

Used to delete data.

```http
DELETE /users/1
```

---

# 8. What is HTTPS?

HTTPS stands for:

**HyperText Transfer Protocol Secure**

It is a secure version of HTTP.

HTTPS uses SSL/TLS encryption to protect data during transmission.

### Without HTTPS

Sensitive data like passwords can be intercepted.

### With HTTPS

Data is encrypted and secure.

### Example

Secure:

```text
https://google.com
```

Not Secure:

```text
http://example.com
```

---

# 9. What is a URL?

URL stands for:

**Uniform Resource Locator**

It is the address of a resource on the Internet.

### Example

```text
https://www.google.com/search?q=mern
```

### URL Components

#### Protocol

```text
https
```

#### Domain

```text
google.com
```

#### Path

```text
/search
```

#### Query Parameter

```text
?q=mern
```

---

# 10. What is Client-Server Architecture?

Modern web applications use Client-Server Architecture.

### Client

The client sends requests.

Examples:

* Browser
* Mobile App

### Server

The server processes requests and sends responses.

Examples:

* Node.js Server
* Express Server

### Architecture

```text
Client
   |
Request
   |
   v
Server
   |
Response
   |
   v
Client
```

---

# How This Relates to MERN Stack

### Frontend

React.js

```text
Client
```

### Backend

Node.js + Express.js

```text
Server
```

### Database

MongoDB

Stores application data.

### Complete MERN Flow

```text
React
   |
   v
Node.js
   |
   v
Express.js
   |
   v
MongoDB
```

---

# Interview Questions

## 1. What is DNS?

DNS (Domain Name System) converts domain names into IP addresses so that computers can locate servers on the Internet.

---

## 2. What happens when you enter a URL in the browser?

1. Browser reads the URL
2. DNS lookup occurs
3. IP address is found
4. Request is sent to server
5. Server processes request
6. Response is returned
7. Browser renders the webpage

---

## 3. Difference Between HTTP and HTTPS?

| HTTP          | HTTPS     |
| ------------- | --------- |
| Not Secure    | Secure    |
| No Encryption | Encrypted |
| Port 80       | Port 443  |

---

## 4. What is an IP Address?

An IP Address is a unique identifier assigned to a device connected to a network.

---

## 5. What is a Browser?

A Browser is software used to access and display websites.

---

## 6. What is a Server?

A Server is a computer that stores data and provides services to clients.

---

## 7. What is Client-Server Architecture?

A model where clients send requests and servers process those requests and return responses.

---

# Summary

* Internet is a network of connected devices.
* Browsers help us access websites.
* Servers store and provide data.
* DNS converts domain names into IP addresses.
* HTTP is used for communication between client and server.
* HTTPS provides secure communication.
* URLs identify resources on the Internet.
* Modern applications follow Client-Server Architecture.
* MERN applications use React, Node.js, Express.js, and MongoDB together.

---

# GitHub Commit Message

```bash
git add .
git commit -m "Day 02: Learned Internet, Browsers, DNS, HTTP/HTTPS and Client-Server Architecture"
git push
```

---

## Next Day Topic

**Day 03 - HTML Fundamentals & Structure of a Web Page**

Topics:

* Introduction to HTML
* HTML Document Structure
* Elements and Tags
* Headings
* Paragraphs
* Links
* Images
* Lists
* Tables
* Forms
* Semantic HTML
