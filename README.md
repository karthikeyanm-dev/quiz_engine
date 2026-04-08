# 🎯 Quiz Engine — Core Java + JDBC

A **console-based Quiz Application** built using **Core Java + JDBC**, designed to demonstrate real-world backend concepts like **OOP, Collections, Database Interaction, Transactions, and Layered Architecture**.

---

## 🚀 Features

- 👤 User Registration & Login  
- 📚 Database-driven Question Bank  
- 🎮 Interactive Quiz Sessions  
- 🧮 Scoring System (based on difficulty)  
- 🏆 Leaderboard (Top 10 Players)  
- 📊 Quiz History Tracking  
- 🔐 JDBC with PreparedStatement (SQL Injection Safe)  
- 🔁 Transaction Management (Atomic DB operations)

---

## 🛠 Tech Stack

- Java (Core Java, OOP)
- JDBC
- MySQL
- Maven

---

## 📁 Project Structure

```
quiz-engine/
│
├── src/
│   ├── model/        # Entities (User, Question, QuizResult, Difficulty)
│   ├── db/           # DB Config & Setup
│   ├── dao/          # Database Operations
│   ├── service/      # Business Logic
│   ├── exception/    # Custom Exceptions
│   └── main/         # Entry Point (QuizApp.java)
│
└── pom.xml           # Dependencies
```

---

## ⚙️ Prerequisites

Make sure you have:

- Java 8 or higher
- MySQL installed
- Maven installed
- IDE (IntelliJ / Eclipse / VS Code)

---

## 🧑‍💻 Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/quiz-engine.git
cd quiz-engine
```

---

### 2️⃣ Configure Database

Open:

```
src/db/DatabaseConfig.java
```

Update credentials:

```java
private static final String URL = "jdbc:mysql://localhost:3306/quiz_engine";
private static final String USER = "root";
private static final String PASS = "yourpassword";
```

---

### 3️⃣ Create Database & Tables

Run the application once OR manually execute:

```sql
CREATE DATABASE quiz_engine;
USE quiz_engine;
```

Tables will be auto-created using:

```java
DatabaseSetup.createTables();
```

---

### 4️⃣ Add MySQL Dependency (pom.xml)

```xml
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
    <version>8.0.33</version>
</dependency>
```

---

### 5️⃣ Run the Application

Run:

```
QuizApp.java
```

---

## 🎮 How to Use

### 🔐 Authentication Menu

```
1. Register
2. Login
3. View Leaderboard
0. Exit
```

---

### 🧠 Quiz Flow

1. Login/Register  
2. Choose Category (Java / DBMS / General)  
3. Answer 5 Questions  
4. Get Score + Grade  
5. View Leaderboard  

---

## 🧮 Scoring System

| Difficulty | Points |
|----------|--------|
| EASY     | +5     |
| MEDIUM   | +10    |
| HARD     | +15    |

---

## 🏗 Core Concepts Covered

- OOP (Encapsulation, Classes, Enums)
- Collections (List, Map)
- JDBC (Connection, PreparedStatement, ResultSet)
- Transactions (Commit / Rollback)
- Exception Handling (Custom Exceptions)
- Layered Architecture (DAO → Service → Main)

---

## 🔥 Sample Output

```
QUIZ STARTED — Category: Java

Q1: What does JVM stand for?
A) Java Virtual Machine
B) Java Variable Method
...

✅ Correct! +5 points

QUIZ COMPLETE!
Score: 40
Grade: A
🏆 NEW HIGH SCORE!
```

---

## 🚀 Future Improvements

- 🔐 Password Hashing (BCrypt)
- ⏱ Timer-based Quiz
- 🌐 REST API (Spring Boot)
- 📱 UI Version (Web/App)
- 🧪 Unit Testing (JUnit)
- 👨‍💼 Admin Panel

---

## 🧑‍🎓 Learning Outcome

By completing this project, students will:

- Understand real-world backend architecture
- Gain hands-on experience with JDBC
- Learn transaction handling
- Build scalable Java applications

---

## 🤝 Contribution

Feel free to fork and improve this project!

---

## 📌 Author

**Karthikeyan M**
