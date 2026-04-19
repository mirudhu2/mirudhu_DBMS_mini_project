# Courier Management System (Java + MySQL)

A complete **Courier Management System** built using **Java**, **Swing GUI**, **JDBC**, and **MySQL**.
This project provides both:
* **GUI Application** using Java Swing
* **Console-Based Application** using Java Scanner

It allows managing:
* Customers
* Couriers
* Employees
* Courier Status Updates
* Record Deletion

# Features

## GUI Version (`CourierGUI.java`)
Modern tab-based interface with:

### Customers Module
* Add Customer
* View Customers
* Update Customer
* Delete Customer

### Couriers Module
* Add Courier
* View Couriers
* Update Courier Details
* Delete Courier
  
### Employees Module
* Add Employee
* View Employees
* Update Employee
* Delete Employee

## Console Version (`CourierFinal.java`)
Menu-driven terminal application with options:
1. Add Customer
2. Add Courier
3. View Customers
4. View Couriers
5. Add Employee
6. View Employees
7. Update Courier Status
8. Delete Courier
9. Exit

# Technologies Used
* Java
* Java Swing
* JDBC
* MySQL Database
* OOP Concepts

# Database Setup
Create a database named:
CREATE DATABASE courier_db;
USE courier_db;
## Customers Table
CREATE TABLE customers (
    customer_id VARCHAR(20) PRIMARY KEY,
    name VARCHAR(50),
    phone VARCHAR(20),
    address VARCHAR(100)
);
## Couriers Table
CREATE TABLE couriers (
    courier_id VARCHAR(20) PRIMARY KEY,
    sender_id VARCHAR(20),
    receiver_id VARCHAR(20),
    weight DOUBLE,
    status VARCHAR(30)
);
## Employees Table
CREATE TABLE employees (
    emp_id VARCHAR(20) PRIMARY KEY,
    name VARCHAR(50),
    role VARCHAR(50),
    phone VARCHAR(20)
);

# Database Connection
Update your MySQL credentials inside Java files:
static final String DB_URL = "jdbc:mysql://localhost:3306/courier_db";
static final String USER = "root";
static final String PASS = "dbms";

# How to Run

## Step 1: Add MySQL JDBC Driver
Download MySQL Connector JAR and add it to project libraries.
## Step 2: Run Console Version
javac CourierFinal.java
java CourierFinal
## Step 3: Run GUI Version
javac CourierGUI.java
java CourierGUI

# Sample Output

## Console Menu
--- Courier Management System ---
1. Add Customer
2. Add Courier
3. View Customers
4. View Couriers
5. Add Employee
6. View Employees
7. Update Courier Status
8. Delete Courier
9. Exit

# Future Improvements
* Login Authentication
* Search Courier by ID
* Delivery Tracking
* Billing System
* Reports Generation
* Better UI Design

# Author
Developed using Java + MySQL for DBMS Mini Project.

