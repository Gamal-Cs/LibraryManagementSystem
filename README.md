# Library Management System

## Overview
The **Library Management System** is a desktop application built using Java (Swing) in **NetBeans** and MySQL as the backend database. It provides essential functionalities to manage books and staff efficiently.

## Features
### **Front End:**
- Developed in **NetBeans** using **Java Swing**.
- User-friendly graphical interface.

### **Functions:**
- **Login Page** – Secure access for administrators.
- **Books Available** – View available books in the library.
- **Staff Details** – Manage staff records.
- **Add Books** – Add new books to the collection.
- **Remove Books** – Remove books from the system.
- **Add Staff** – Register new staff members.
- **Remove Staff** – Delete staff records.

### **Back End:**
- **Database:** MySQL
- **Tables:** Admin, Books, and Staff

## Database Schema
Use the following SQL queries to create the required tables:

```sql
CREATE TABLE ADMIN (
    USER_ID VARCHAR(50) PRIMARY KEY,
    NAME VARCHAR(50),
    PASSWORD VARCHAR(50),
    CONTACT VARCHAR(10)
);

CREATE TABLE BOOKS (
    BOOK_ID VARCHAR(50) PRIMARY KEY,
    CATEGORY VARCHAR(50),
    NAME VARCHAR(50),
    AUTHOR VARCHAR(50),
    COPIES INT
);

CREATE TABLE STAFFS (
    STAFF_ID VARCHAR(50) PRIMARY KEY,
    NAME VARCHAR(50),
    CONTACT VARCHAR(50)
);
```

## How to Run the Project

### **1. Set Up the Database**
- Install MySQL and create a database.
- Execute the SQL queries above to create the necessary tables.

### **2. Configure Database Connection**
- Open the project in **NetBeans**.
- Locate the `Conn.getConnection()` method in your project.
- Update it with your MySQL credentials (database name, username, and password).

### **3. Run the Project**
- Open the project in **NetBeans**.
- Compile and run the project.
- Test the available features.

## Requirements
- **NetBeans IDE**
- **Java Development Kit (JDK)**
- **MySQL Database Server**
- **JDBC Driver for MySQL**

## Author
- Developed by **Gamal-Cs**
