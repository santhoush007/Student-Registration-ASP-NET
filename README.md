# 🎓 Student Registration System

A web-based application built with **ASP.NET (C#)** and **ADO.NET** to manage student registrations. This project demonstrates the implementation of a **Connected/Disconnected Architecture** using **Microsoft SQL Server** as the backend.

---

## 🚀 Features
* **Student Registration Form:** Captures Name, Course, Cell No, and Email.
* **Database Integration:** Stores data securely in MS SQL Server.
* **Validation:** Basic input validation included.
* **Architecture:** Uses ADO.NET for efficient data handling.

---

## 🛠️ Tech Stack
* **Frontend:** ASP.NET Web Forms (.aspx), HTML, CSS
* **Backend:** C# (.NET Framework)
* **Database:** Microsoft SQL Server (LocalDB / Express)
* **Data Access:** ADO.NET (SqlClient)
* **IDE:** Visual Studio

---

## ⚙️ How to Run Locally

### 1. Database Setup
Execute the following SQL script in your **SQL Server Management Studio (SSMS)** to create the database and table:

```sql
CREATE DATABASE CollegeDB;
GO
USE CollegeDB;
GO

CREATE TABLE StudentReg (
    StudentID INT IDENTITY(1,1) PRIMARY KEY,
    Name NVARCHAR(100),
    CourseName NVARCHAR(100),
    CellNo NVARCHAR(15),
    EmailId NVARCHAR(100)
);
