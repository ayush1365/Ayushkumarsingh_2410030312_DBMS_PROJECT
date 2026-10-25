# 🏥 Hospital Management System

**DBMS Minor Project | MySQL | IILM University, Greater Noida**

This repository contains the documentation, presentation, SQL implementation, and project report for the **Hospital Management System**, developed as part of the Database Management Systems (DBMS) minor project for the academic session **2025–2026**.

---

## 👤 Student Details

| **Field** | **Details** |
|---|---|
| **Name** | Ayush Kumar Singh |
| **Roll Number** | 2410030312 |
| **Institute** | IILM University, Greater Noida, Uttar Pradesh |
| **Programme** | B.Tech Computer Science and Engineering |
| **Class** | 2CSE2 |
| **Course Code** | UCS4001 |
| **Project Type** | DBMS Minor Project |
| **Academic Session** | 2025–2026 |
| **Database** | Hospitalmanagement |
| **Technology** | MySQL |

---

## 📌 About the Project

The **Hospital Management System** is a database-based project designed to manage essential hospital operations in an organised and structured manner.

The system maintains information about patients, doctors, hospital staff, rooms, appointments, admissions, medicines, prescriptions, and billing. It uses MySQL to store and manage records through SQL queries.

The project demonstrates the practical application of database management concepts, including table creation, primary keys, foreign keys, constraints, data insertion, and relationships between tables.

---

## 🎯 Project Objectives

- Maintain organised patient and doctor records.
- Manage hospital appointments and admissions.
- Store information about medicines and prescriptions.
- Maintain room availability and room charges.
- Record billing details and payment status.
- Reduce unnecessary data redundancy.
- Understand relational database design and normalisation.
- Practise SQL commands and database operations.

---

## 🛠️ Technologies & Tools Used

`MySQL` · `SQL` · `Relational Database Management System` · `Primary Keys` · `Foreign Keys` · `Database Design`

### MySQL
Used to create the `Hospitalmanagement` database, define tables, store records, and execute SQL queries.

### SQL
Used for database creation, table definition, data insertion, and retrieving or managing records.

### Relational Database Concepts
Used to organise information into related tables and establish relationships through primary and foreign keys.

---

## 🗄️ Database Structure

**Database Name:** `Hospitalmanagement`

The project contains nine main tables:

| **Table** | **Purpose** |
|---|---|
| `Patient` | Stores patient details such as name, age, gender, phone, and address. |
| `Doctor` | Stores doctor names, specialisations, and phone numbers. |
| `Staff` | Maintains staff details, roles, and phone numbers. |
| `Room` | Stores room types, availability status, and charges. |
| `Appointment` | Records patient appointments with doctors, including date and time. |
| `Admission` | Maintains admission, room allocation, and discharge details. |
| `Medicine` | Stores medicine names, prices, and stock quantities. |
| `Prescription` | Records prescribed medicines, patients, doctors, quantities, and dates. |
| `Billing` | Maintains patient bills, amounts, payment status, and bill dates. |

---

## 🔑 Database Relationships

The database uses primary keys to uniquely identify records and foreign keys to connect related tables.

- **Patient → Appointment:** Connects patients with their appointments.
- **Doctor → Appointment:** Connects doctors with scheduled appointments.
- **Patient → Admission:** Links patients to admission records.
- **Room → Admission:** Connects admissions with allocated rooms.
- **Patient → Prescription:** Links prescriptions to patients.
- **Doctor → Prescription:** Identifies the prescribing doctor.
- **Medicine → Prescription:** Connects prescriptions with medicines.
- **Patient → Billing:** Associates billing records with patients.

These relationships help maintain referential integrity between the related tables.

---

## 💻 Database Implementation

### Step 1: Create the Database

```sql
CREATE DATABASE Hospitalmanagement;

USE Hospitalmanagement;
```

### Step 2: Create a Table

Example: Patient table.

```sql
CREATE TABLE Patient (
    PatientID INT PRIMARY KEY,
    Name VARCHAR(50) NOT NULL,
    Age INT,
    Gender VARCHAR(10),
    Phone VARCHAR(15) UNIQUE,
    Address VARCHAR(100)
);
```

### Step 3: Insert Sample Data

```sql
INSERT INTO Patient
VALUES (
    1,
    'Rahul',
    25,
    'Male',
    '9876543210',
    'Noida'
);
```

### Step 4: Retrieve Records

```sql
SELECT * FROM Patient;
```

### Step 5: View Table Structure

```sql
DESC Patient;
```

The same approach is used to create and manage the remaining tables in the database.

---

## ⚙️ Key Features

- **Patient Management:** Store and retrieve patient information.
- **Doctor Management:** Maintain doctor details and specialisations.
- **Appointment Management:** Record appointment dates and times.
- **Admission Management:** Maintain admission and discharge records.
- **Room Management:** Track room types, status, and charges.
- **Medicine Management:** Store medicine prices and stock quantities.
- **Prescription Management:** Associate patients, doctors, and medicines.
- **Billing Management:** Record bill amounts and payment status.

---

## 🔄 Project Workflow

```text
Start
  ↓
Create MySQL Database
  ↓
Create Relational Tables
  ↓
Define Primary & Foreign Keys
  ↓
Insert Sample Data
  ↓
Execute SQL Queries
  ↓
Retrieve and Verify Records
  ↓
End
```

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Creating and managing relational databases using MySQL.
- Designing tables with suitable data types.
- Implementing primary key and foreign key constraints.
- Inserting and retrieving records using SQL.
- Understanding relationships between hospital entities.
- Organising data into separate tables to reduce redundancy.
- Applying DBMS concepts to a practical hospital management scenario.

---

## 📁 Repository Contents

```text
Hospital-Management-System/
│
├── README.md
├── Hospital Management System.dbms.pptx
├── DBMS PROJECT 2CSE2 HOSPITAL MANAGEMENT.pdf
└── SQL/
    └── hospital_management.sql
```

*Note: Update the filenames above to match the actual filenames in your GitHub repository. Add the SQL file only after saving your implementation as `hospital_management.sql`.*

---

## 📄 Project Documentation

The project documentation and presentation cover:

1. Introduction
2. Project Objectives
3. Database Creation
4. Table Structure and Definitions
5. Sample Data Insertion
6. Primary and Foreign Key Relationships
7. Database Operations
8. Output Verification
9. Learning Outcomes

---

## 🙏 Acknowledgement

I would like to express my sincere gratitude to **IILM University, Greater Noida**, and the faculty members of the School of Computer Science and Engineering for providing the opportunity to develop this DBMS minor project.

I am also thankful to my teammates **Aman Kumar Singh, Hardik Tomar, and Keshav Kumar** for their contributions to the Hospital Management System project.

---

## 📌 Project Summary

The Hospital Management System demonstrates how a relational database can be used to organise hospital records and support essential operations such as patient registration, appointments, admissions, medicine management, prescriptions, and billing.

Developed using **MySQL and SQL**, this project strengthened my understanding of relational database design, constraints, table relationships, and practical database operations.

---

**Ayush Kumar Singh** · B.Tech Computer Science and Engineering · IILM University, Greater Noida

**Hospital Management System | DBMS Minor Project | Academic Session 2025–2026**
