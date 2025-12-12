# Library Management System 
---

## Overview
This project implements a fully functional **Library Management System** using **Object-Oriented Programming (OOP)** in Java, built with **Maven**.  
The system allows two types of users:

- **Librarian**
- **Member**

Each user interacts through a clean, menu-driven interface.  
The system ensures proper OOP design using classes such as `Library`, `Book`, `Member`, `Librarian`, and corresponding helper classes.

---

## Features

### Librarian Functionalities
- Add a new book (multiple copies allowed)
- Remove a book
- Register a new member
- Remove a member
- Issue a book to a member
- Collect fines
- View all members with:
  - Their borrowed books
  - Their outstanding fines
- View all books with:
  - Total copies
  - Available copies

### Member Functionalities
- Log in using **name + phone number**
- View available books
- View books they have borrowed
- Issue a book (max 2 books, no dues pending)
- Return a book (fine applied if returned late)
- Pay dues online
- Log out

---

## Fine Calculation
- A member must return a book **within 10 days**.
- **For testing: 1 second = 1 day**
- Fine = **₹3 per day** after the due date.
- Member must clear dues before issuing another book.

---

## How to Compile & Run

### **1. Ensure Maven is installed**
Verify using:
```bash
mvn -v
```

### **2. Compile the project**
```bash
mvn clean compile
```

### **3. Run the application**
```bash
mvn exec:java -Dexec.mainClass="library.Main"
```

---

## Input Validation & Error Handling
- Attempts to borrow more than 2 books → denied
- Returns book not borrowed → error
- Wrong member login → error displayed
- Book ID or Member ID not found → validated
- Member with pending dues cannot issue new books

---

## OOP Concepts Used
- **Encapsulation** → private fields + getters/setters  
- **Classes & Objects** → Book, Member, Library, etc.  
- **Relationships**   
- **Data Hiding & Validation**

---

**Lab Assignment 01**.

