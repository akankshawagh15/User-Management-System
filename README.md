# Java User Management System

This is a simple Java application for managing user information. The application uses a MySQL database to store user details, allowing administrators to perform operations such as adding, editing, and deleting user records.

## Features

- Register a new user with details like name, email, mobile number, date of birth, city, and gender.
- View a list of all registered users.
- Edit existing user details.
- Delete users from the system.

## Technologies Used

- Java
- MySQL
- Servlets and JSP for the web interface
- JDBC for database connectivity

## Prerequisites

- Java Development Kit (JDK)
- MySQL Database
- Apache Tomcat

## Setup Database

1. Create a MySQL database named `usermgmt` for the User Management System.

   ```sql
   CREATE DATABASE usermgmt;
## user table
CREATE TABLE user (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL,
    mobile VARCHAR(20) NOT NULL,
    dob VARCHAR(20) NOT NULL,
    city VARCHAR(255) NOT NULL,
    gender VARCHAR(10) NOT NULL
);
