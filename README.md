# Travel Management System (Java Swing)

A **desktop-based Travel Management System** built using **Java Swing and MySQL**.
This application allows users to manage travel bookings, view travel packages, book hotels, and maintain customer records through an interactive graphical interface.

The project demonstrates **Java GUI development, JDBC database connectivity, and basic database management**, making it suitable for academic learning and beginner-level Java projects.

---

## 📌 Features

* User **Login and Signup system**
* **Customer management**
* **Travel package browsing**
* **Hotel booking system**
* **Package booking system**
* **Payment interface simulation**
* **View and update customer information**
* **Database integration using JDBC**

---

## 🏗️ Project Architecture

The system follows a **three-layer architecture**:

1. **Presentation Layer**

   * Java Swing GUI
   * Handles user interaction

2. **Application Logic Layer**

   * Java classes controlling program flow
   * Processes user requests

3. **Database Layer**

   * MySQL database
   * Stores user data, bookings, and packages

---

## 🧰 Technologies Used

| Technology   | Purpose                        |
| ------------ | ------------------------------ |
| Java         | Core programming language      |
| Java Swing   | GUI development                |
| MySQL        | Database management            |
| JDBC         | Database connectivity          |
| NetBeans IDE | Development environment        |
| rs2xml       | Display database tables in GUI |

---

## 📂 Project Structure

```
TravelManagementSystem
│
├── src/travel/management/system
│   ├── Conn.java
│   ├── Login.java
│   ├── Signup.java
│   ├── Splash.java
│   ├── Home.java
│   ├── BookHotel.java
│   ├── BookPackage.java
│   ├── Payment.java
│   ├── ViewCustomers.java
│   └── UpdateCustomer.java
│
├── icons
│   └── UI images used in the application
│
├── build
├── dist
└── README.md
```

---

## 🗄️ Database Design

The application uses a **MySQL database named `tms`**.

### Tables

**1. Account**
Stores user login information.

| Column   | Description       |
| -------- | ----------------- |
| username | User login name   |
| name     | Full name         |
| password | Account password  |
| security | Security question |
| answer   | Security answer   |

---

**2. Customer**
Stores customer personal information.

| Column   | Description     |
| -------- | --------------- |
| username | Associated user |
| id_type  | ID proof type   |
| number   | ID number       |
| name     | Customer name   |
| gender   | Gender          |
| country  | Country         |
| address  | Address         |
| phone    | Contact number  |
| email    | Email address   |

---

**3. Package**
Stores available travel packages.

| Column      | Description     |
| ----------- | --------------- |
| name        | Package name    |
| duration    | Trip duration   |
| price       | Package price   |
| description | Package details |

---

**4. BookPackage**
Stores package booking information.

---

**5. Hotel**
Stores hotel details.

---

**6. BookHotel**
Stores hotel booking records.

---

## ⚙️ Installation and Setup

### 1. Clone the repository

```
git clone https://github.com/yourusername/travel-management-system-java.git
```

---

### 2. Install Requirements

Make sure you have:

* Java JDK (17 or higher)
* MySQL Server
* NetBeans IDE

---

### 3. Create Database

Open MySQL and run:

```
CREATE DATABASE tms;
USE tms;
```

Create required tables according to the database schema.

---

### 4. Configure Database Connection

Open `Conn.java` and update your database credentials:

```
Connection c = DriverManager.getConnection(
"jdbc:mysql://localhost:3306/tms",
"root",
"yourpassword"
);
```

---

### 5. Add Required Libraries

Add the following libraries to your project:

* `mysql-connector-j.jar`
* `rs2xml.jar`

---

### 6. Run the Application

Run:

```
Splash.java
```

The application will start with the **login interface**.

---

## 🔑 Default Login Credentials

Example account:

```
Username: admin
Password: 1234
```

---

## 🖥️ Application Workflow

1. Splash Screen
2. Login / Signup
3. Home Dashboard
4. Book Travel Packages
5. Book Hotels
6. Manage Customer Details
7. Payment Interface

---

## 🎯 Learning Objectives

This project helps understand:

* Java GUI development with Swing
* Database connectivity using JDBC
* CRUD operations in MySQL
* Desktop application design
* Event-driven programming in Java

---

## 🚀 Future Improvements

Possible enhancements include:

* Online payment gateway integration
* REST API backend
* Web-based version using Spring Boot
* Role-based access control
* Secure password hashing
* Deployment as a cloud application

---

## 👨‍💻 Author

**Alvin Boby**

Computer Science Engineering Student
Interested in **Cybersecurity, Cryptography, and Secure Systems Development**

---

## 📜 License

This project is for **educational and learning purposes**.
