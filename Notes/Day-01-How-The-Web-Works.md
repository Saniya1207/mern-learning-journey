# Day 01 - How The Web Works

## Introduction

Before learning MERN Stack, it is important to understand how the internet and websites work.

Every web application, whether it is Instagram, Amazon, LinkedIn, or a MERN application, follows the same fundamental process:

User → Browser → Server → Database → Server → Browser

---

# What is a Website?

A website is a collection of interconnected web pages hosted on a server and accessible through the internet.

Examples:

- Google
- Amazon
- YouTube
- Netflix
- Facebook

A website consists of:

1. Frontend
2. Backend
3. Database

---

# What Happens When We Enter a URL?

Example:

https://www.google.com

When a user enters a URL, the following steps occur:

### Step 1: DNS Lookup

The browser asks the DNS (Domain Name System):

"Where is google.com located?"

DNS converts the domain name into an IP address.

Example:

google.com → 142.250.xxx.xxx

---

### Step 2: Browser Sends Request

The browser sends an HTTP request to the server.

Example:

GET / HTTP/1.1

The request asks the server for data.

---

### Step 3: Server Processes Request

The server receives the request.

The backend application:

- Validates request
- Executes business logic
- Communicates with database

---

### Step 4: Database Operations

If data is required:

Server → Database

Database → Server

Example:

User requests profile information.

Server fetches data from MongoDB.

---

### Step 5: Server Sends Response

The server returns an HTTP response.

Example:

200 OK

Response may contain:

- HTML
- JSON
- Images
- Videos

---

### Step 6: Browser Displays Result

The browser renders the response and displays the webpage.

The user sees the final output.

---

# Client

A client is a device or application that requests data.

Examples:

- Chrome Browser
- Firefox Browser
- Mobile App
- React Application

Responsibilities:

- Sending requests
- Displaying data
- Handling user interactions

---

# Server

A server is a computer or software that processes requests and provides responses.

Examples:

- Node.js Server
- Express Server
- Apache Server
- Nginx Server

Responsibilities:

- Authentication
- Business Logic
- Database Communication
- API Handling

---

# Frontend

Frontend is everything visible to the user.

Examples:

- Buttons
- Forms
- Images
- Navigation Bar
- Dashboard

Technologies:

- HTML
- CSS
- JavaScript
- React.js

Frontend is responsible for User Interface (UI).

---

# Backend

Backend is the hidden part of an application.

Responsibilities:

- Authentication
- Authorization
- Database Operations
- Business Logic
- API Creation

Technologies:

- Node.js
- Express.js
- PHP
- Python
- Java

---

# Database

A database stores information permanently.

Examples:

- User Data
- Orders
- Products
- Messages

Popular Databases:

### SQL Databases

- MySQL
- PostgreSQL

### NoSQL Databases

- MongoDB

---

# What is an API?

API stands for:

Application Programming Interface

An API acts as a bridge between Frontend and Backend.

Example:

React Application

↓

Request

↓

Node.js API

↓

MongoDB Database

↓

Response

↓

React Application

---

# HTTP Methods

## GET

Used to fetch data.

Example:

Get all products.

---

## POST

Used to create data.

Example:

Create new user.

---

## PUT

Used to update existing data.

Example:

Update profile.

---

## DELETE

Used to remove data.

Example:

Delete product.

---

# MERN Stack Overview

MERN stands for:

## M - MongoDB

Database used to store data.

---

## E - Express.js

Backend framework for Node.js.

---

## R - React.js

Frontend library used to build user interfaces.

---

## N - Node.js

JavaScript runtime used to run JavaScript outside the browser.

---

# MERN Architecture

React (Frontend)

↓

Express.js (Backend)

↓

Node.js (Runtime)

↓

MongoDB (Database)

---

# Real Life Example

Instagram Login

Step 1:
User enters email and password.

Step 2:
React sends request.

Step 3:
Node.js + Express receives request.

Step 4:
MongoDB verifies credentials.

Step 5:
Server generates response.

Step 6:
React displays dashboard.

---

# Interview Questions

## What is DNS?

DNS converts domain names into IP addresses.

---

## What is a Client?

A client is a device or application that requests data from a server.

---

## What is a Server?

A server processes requests and returns responses.

---

## What is an API?

An API allows communication between frontend and backend systems.

---

## Difference Between Frontend and Backend?

Frontend:
Visible to users.

Backend:
Handles logic and database operations.

---

## What Does MERN Stand For?

MongoDB
Express.js
React.js
Node.js

---

# Key Takeaways

- Every web application follows Client → Server → Database architecture.
- Frontend handles UI.
- Backend handles logic.
- Database stores information.
- APIs connect frontend and backend.
- MERN Stack consists of MongoDB, Express.js, React.js and Node.js.
- Understanding web architecture is essential before learning React and Node.js.

---

# Day 01 Status

✅ Completed

Next Topic:

Day 02 - JavaScript Fundamentals for MERN Development
