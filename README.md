# FCC-Worldcup-database

# ⚽ World Cup Database Project

A PostgreSQL database project built as part of the freeCodeCamp Relational Database Certification. This project stores World Cup teams and match data, and performs various SQL queries to analyze tournament statistics.

---

## 📌 Features

✅ Create and manage a PostgreSQL database  
✅ Store World Cup match and team information  
✅ Insert data automatically using Bash scripting  
✅ Run analytical SQL queries  
✅ Use relational database concepts like:
- Primary Keys
- Foreign Keys
- Constraints
- Joins
- Aggregate Functions

---

## 🛠️ Technologies Used

- 🐘 PostgreSQL
- 🐚 Bash Scripting
- 💻 SQL
- 🐧 Linux Terminal

---

## 📂 Project Files

### 📄 `insert_data.sh`
Reads data from `games.csv` and inserts:
- Teams into the `teams` table
- Match details into the `games` table

---

### 📄 `queries.sh`
Contains SQL queries to retrieve:
- Total goals
- Average goals
- Tournament champions
- Team statistics
- Match statistics

---

### 📄 `worldcup.sql`
Database dump file containing:
- Database creation
- Table creation
- Constraints
- Insert statements
- Foreign keys

---

## 🗄️ Database Schema

### 🏆 Teams Table

| Column | Type |
|--------|------|
| `team_id` | SERIAL PRIMARY KEY |
| `name` | VARCHAR(255) UNIQUE NOT NULL |

---

### ⚽ Games Table

| Column | Type |
|--------|------|
| `game_id` | SERIAL PRIMARY KEY |
| `year` | INT NOT NULL |
| `round` | VARCHAR(255) NOT NULL |
| `winner_id` | INT NOT NULL |
| `opponent_id` | INT NOT NULL |
| `winner_goals` | INT NOT NULL |
| `opponent_goals` | INT NOT NULL |

---

🎯 Learning Outcomes
Working with relational databases
Writing SQL queries
Using Bash with PostgreSQL
Database normalization
Data import/export
Query optimization basics

👩‍💻 Author: Poulami Sarkar

📜 Built for the freeCodeCamp Relational Database Certification Program.
