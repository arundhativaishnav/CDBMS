# 🗃️ Customised Database Management System (DBMS) in Java

A simple, console-based **Database Management System** implemented using core Java and a singly linked list. This project simulates basic SQL operations like **Insert, Select, Update, Delete**, and aggregate functions like **Count, Sum, Avg, Max, Min** — all without using a real database.

---

## 📌 Features

- Insert new student records
- Display all student records
- Filter records based on city or name
- Count total records
- Compute:
  - Sum of marks
  - Average of marks
  - Maximum marks
  - Minimum marks
- Update city by roll number
- Delete student record by roll number

---

## 💻 Technologies Used

- Java (Core Java)
- Object-Oriented Programming
- Data Structures (Singly Linked List)

---

## 📂 Project Structure

- `cdbms.java`: Entry point and testing of all DBMS operations
- `DBMS.java`: Core database logic (Insert, Select, Delete, etc.)
- `node.java`: Represents one student record (row in the table)

---

## 🔄 Supported Queries (Simulated)

| SQL Query (Equivalent)                                 | Method in Code                      |
|--------------------------------------------------------|-------------------------------------|
| `INSERT INTO student VALUES('Amit','Pune',78);`        | `InsertIntoTable("Amit","Pune",78)` |
| `SELECT * FROM student;`                               | `SelectStarFrom()`                  |
| `SELECT * FROM student WHERE City = 'Pune';`           | `SelectStarFromWhereCity("Pune")`   |
| `SELECT * FROM student WHERE Name = 'Amit';`           | `SelectStarFromWhereName("Amit")`   |
| `SELECT COUNT(Marks) FROM student;`                    | `SelectCount()`                     |
| `SELECT SUM(Marks) FROM student;`                      | `SelectSum()`                       |
| `SELECT AVG(Marks) FROM student;`                      | `SelectAvg()`                       |
| `SELECT MAX(Marks) FROM student;`                      | `SelectMax()`                       |
| `SELECT MIN(Marks) FROM student;`                      | `SelectMin()`                       |
| `UPDATE student SET City = 'Nashik' WHERE Rno = 3;`    | `UpdateCity(3, "Nashik")`           |
| `DELETE FROM student WHERE Rno = 5;`                   | `DeleteFrom(5)`                     |

---

## 📝 Sample Output
DBMS initialised successfully
Student table gets created successfully...
One record gets inserted successfully
Data from the student table is :
1 Amit Pune 89
2 Pooja Mumbai 95
...
Average of Marks column is : 86.4
Maximum from Marks column is : 95
Minimum from Marks column is : 78

## 🛠️ How to Run

1. Make sure Java is installed.
2. Compile the program
3. Run the program


## 📘 Learning Outcomes

- Understanding how databases work internally
- Implementing table-like structures using linked lists
- Simulating SQL-like commands using object-oriented design
- Practicing CRUD operations programmatically
