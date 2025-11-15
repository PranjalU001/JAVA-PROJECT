# JAVA-PROJECT
Here is a clean, professional **README.md** for your project based on the content you provided:

---

# Spring Boot + Hibernate (Native) + MySQL Web Application

This project is a **CRUD-based web application** built using **Spring Boot**, **Native Hibernate** (without JPA), and **MySQL**.
The goal is to demonstrate how to build a fully functional web application using Hibernate’s native APIs instead of JPA-specific methods.

---

## 🛠️ Tools & Technologies Used

| Technology      | Version        |
| --------------- | -------------- |
| **Java**        | 1.8            |
| **Spring Boot** | 2.1.1          |
| **Hibernate**   | 5.3.7          |
| **MySQL**       | 8.0.13         |
| **IDE**         | Eclipse Oxygen |

---

## 🚀 Steps to Install & Run the Application

### **1. Clone the Repository**

```bash
git clone https://github.com/......
```

--

### **2. Create MySQL Database**

Run the following SQL command:

```sql
CREATE DATABASE crudapi;
```

---

### **3. Create Table (or Run SQL Script)**

```sql
USE crudapi;

CREATE TABLE tbl_employee
(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    gender VARCHAR(255),
    department VARCHAR(255),
    dob DATE
);
```

---

### **4. Update MySQL Credentials**

Open:

```
src/main/resources/application.properties
```

Update the following values as per your system:

```properties
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
```

---

### **5. Run the Application**

#### **Option 1 — Using Maven**

```bash
mvn spring-boot:run
```

#### **Option 2 — Create Jar and Run**

```bash
mvn package
java -jar target/springbootcrudapi-0.0.1-SNAPSHOT.jar
```

---

## 🌐 Application URL

The server will start on:

```
http://localhost:8080
```

---

