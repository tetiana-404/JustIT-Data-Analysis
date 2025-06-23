# JustIT Data Analysis Training – Week 3

This repository contains learning materials and tasks completed during Week 3 of the JustIT training programme. The main focus of this week was understanding database fundamentals, SQL joins, and designing and querying a real-world relational database.

---

## 🧩 Day 1: Database Fundamentals

### Task 1: Database Keys & Relationships

**Key Concepts:**
- **Primary Key**: Uniquely identifies each record.
- **Secondary Key**: Alternate searchable field.
- **Foreign Key**: References a primary key in another table.


**Real-World Relationship Examples:**
- One-to-One → Person and Passport
- One-to-Many → Customer and Orders
- Many-to-Many → Students and Courses

---

### Task 2: Relational vs Non-Relational Databases

- The difference between a relational and nonrelational database

| Feature             | Relational                         | Non-Relational                   |
|---------------------|------------------------------------|----------------------------------|
| Schema              | Fixed                              | Flexible or schema-less          |
| Data Structure      | Rows and columns                   | JSON, key-value, graph, documents|
| Best For            | Structured data                    | Unstructured/semi-structured data|
| Examples            | MySQL, PostgreSQL                  | MongoDB, Firebase, Cassandra     |

---

## 🔗 Day 3: SQL JOIN Types


| JOIN Type     | Description                                  | Use Case Example                          |
|---------------|-----------------------------------------------|-------------------------------------------|
| INNER JOIN    | Returns matching rows from both tables        | Customer Orders                           |
| LEFT JOIN     | All rows from left + matching from right      | All products including unsold             |
| RIGHT JOIN    | All rows from right + matching from left      | All employees including unassigned ones   |
| FULL JOIN     | All matching and unmatched rows from both     | Mailing list combination                  |
| SELF JOIN     | A table joined with itself                    | Employee–Manager structure                |
| CROSS JOIN    | All possible combinations (Cartesian Product) | Product promotions by region              |


---

## 🏪 Day 4: Task 1 – Retail Database Design

**Scenario:** A small retail store wants a system to manage products, customers, sales, and loyalty cards.

**Process:**
1. **Understanding the Business Requirements**
2. **Designing the Database Schema**
3. **Implementing the Database** 
4. **Populating the Database**
5. **Maintaining the Database**
6. **Conclusion**


📄 See full write-up in `Day_4_Retail_Database_Design_Essay.docx`

---

## 💻 Day 4: Task 2 – SQL Practical: `world_db`

**Objective:**  
Apply SQL to query real-world demographic and geographic data from the `world_db` database.

**SQL Tasks:**
1. Count cities in USA 
2. Country with highest life expectancy
3. Cities with "New" in name
4. Display first 10 rows
5. Cities with population > 2,000,000
6. Cities beginning with 'Be'
7. Population between 500,000–1,000,000
8. Cities sorted by name (ascending)
9. Most populated city
10. Count of cities with same name (frequency)
11. City with lowest population
12. Country with largest population
13. Capital of Spain
14. Cities in Europe
15. Average population by country
16. Compare capital cities' population
17. Countries with low population density
18. Cities with high GDP per capita (if GDP data present)
19. Display rows 31–40

📸 *Screenshots and results stored in `Day_4_Task_2_SQL Practical.doc`*


---



