# JustIT Data Analysis Training – Week 3

This repository contains learning materials and tasks completed during Week 3 of the JustIT training programme. The main focus of this week was understanding database fundamentals, SQL joins, and designing and querying a real-world relational database.

---

## 🧩 Day 1: Database Fundamentals

### Task 1: Database Keys & Relationships

**Key Concepts:**
- **Primary Key**
- **Secondary Key**
- **Foreign Key**

**Real-World Relationship Examples:**
- One-to-One 
- One-to-Many 
- Many-to-Many 

---

### Task 2: Relational vs Non-Relational Databases

- The difference between a relational and nonrelational database

---

## 🔗 Day 3: SQL JOIN Types


- INNER JOIN   
- LEFT JOIN  
- RIGHT JOIN  
- FULL JOIN  
- SELF JOIN  
- CROSS JOIN  

---

## 🏪 Day 4: Task 1 – Retail Database Design

**Scenario:** A corner shop wants a system to manage products, customers, sales, and loyalty cards.

**Process:**
1. **Entities Identified**: `Customers`, `Sales`, `Products`, `LoyaltyCards`, `Inventory`
2. **Relationships Defined**:
   - One-to-Many (Customer–Sales)
   - One-to-One (Customer–LoyaltyCard)
3. **Tables Normalised** to reduce redundancy.
4. **Future-Proofing**: Ready for expansion and reporting needs.

📄 See full write-up in `Day_4_Retail_Database_Design_Essay.docx`

---

## 💻 Day 4: Task 2 – SQL Practical: `world_db`

**Objective:**  
Apply SQL to query real-world demographic and geographic data from the `world_db` database.

**Setup Instructions:**
- Download `world_db(1)` dataset
- Create database following setup guide provided
- Run the queries below and include both SQL syntax and output

**SQL Tasks:**

| #  | Task Description                                                   | SQL Function Example                      |
|----|--------------------------------------------------------------------|-------------------------------------------|
| 1  | Count cities in USA                                                | `SELECT COUNT(*) FROM city WHERE CountryCode = 'USA';` |
| 2  | Country with highest life expectancy                               | `SELECT Name FROM country ORDER BY LifeExpectancy DESC LIMIT 1;` |
| 3  | Cities with "New" in name                                          | `SELECT * FROM city WHERE Name LIKE 'New%';` |
| 4  | Display first 10 rows                                              | `SELECT * FROM city LIMIT 10;`            |
| 5  | Cities with population > 2,000,000                                 | `SELECT * FROM city WHERE Population > 2000000;` |
| 6  | Cities beginning with 'Be'                                         | `SELECT * FROM city WHERE Name LIKE 'Be%';` |
| 7  | Population between 500,000–1,000,000                               | `SELECT * FROM city WHERE Population BETWEEN 500000 AND 1000000;` |
| 8  | Cities sorted by name (ascending)                                  | `SELECT * FROM city ORDER BY Name ASC;`   |
| 9  | Most populated city                                                | `SELECT * FROM city ORDER BY Population DESC LIMIT 1;` |
| 10 | Count of cities with same name (frequency)                         | `SELECT Name, COUNT(*) FROM city GROUP BY Name HAVING COUNT(*) > 1;` |
| 11 | City with lowest population                                        | `SELECT * FROM city ORDER BY Population ASC LIMIT 1;` |
| 12 | Country with largest population                                    | `SELECT Name FROM country ORDER BY Population DESC LIMIT 1;` |
| 13 | Capital of Spain                                                   | `SELECT Name FROM city WHERE ID = (SELECT Capital FROM country WHERE Name = 'Spain');` |
| 14 | Cities in Europe                                                   | `SELECT Name FROM city JOIN country ON city.CountryCode = country.Code WHERE continent = 'Europe';` |
| 15 | Average population by country                                      | `SELECT CountryCode, AVG(Population) FROM city GROUP BY CountryCode;` |
| 16 | Compare capital cities' population                                 | `SELECT city.Name, city.Population FROM city JOIN country ON city.ID = country.Capital;` |
| 17 | Countries with low population density                              | `SELECT Name FROM country WHERE Population / SurfaceArea < 50;` |
| 18 | Cities with high GDP per capita (if GDP data present)              | `-- hypothetical query, based on schema`  |
| 19 | Display rows 31–40                                                 | `SELECT * FROM city LIMIT 10 OFFSET 30;`  |

📸 *Screenshots and results stored in `/screenshots/sql_practice_day4_task2/`*

---



