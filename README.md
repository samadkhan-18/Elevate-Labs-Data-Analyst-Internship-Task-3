# Elevate-Labs-Data-Analyst-Internship-Task-3
## Task 3: SQL for Data Analysis

Data Analyst Internship, Elevate Labs

## Objective
Use SQL queries to extract and analyze data from a database.

## Tools Used
- MySQL Server
- MySQL Workbench

## Dataset
`parks_and_recreation` database with three tables:
- `employee_demographics` (employee_id, first_name, last_name, age, gender, birth_date)
- `employee_salary` (employee_id, first_name, last_name, occupation, salary, dept_id)
- `parks_departments`

## What I Did
| Concept | Description |
|---|---|
| SELECT | Retrieved all records from the demographics table |
| WHERE | Filtered employees by gender and salary |
| Subquery | Filtered employees using a nested query on salary |
| GROUP BY | Grouped employees by gender |
| ORDER BY | Sorted employees by first name and by multiple columns |
| INNER JOIN | Combined demographics and salary tables on `employee_id` |
| LEFT / RIGHT JOIN | Showed unmatched rows from either table (NULL values) |
| Aggregate functions | Used AVG, COUNT, MIN, MAX on age grouped by gender |
| VIEW | Created `emp_avg1` view for average age by gender |
| Indexing / optimization | Explored sorting on multiple columns and index usage |

## Repository Contents
- `SQL-DataAnalysis.sql`: all SQL queries
- `screenshots/`: output screenshots from MySQL Workbench
- `README.md`: this file

## Key Observations
- Female employees: 4, average age 38.5 (min 29, max 46)
- Male employees: 7, average age 41.29 (min 34, max 61)
- LEFT JOIN vs RIGHT JOIN showed that Ron Swanson exists in the salary table but not in the demographics table (NULLs appear).

## How to Run
1. Open MySQL Workbench and load the `parks_and_recreation` database.
2. Open `SQL-DataAnalysis.sql`.
3. Run the queries one by one.

## Outcome
Learned to manipulate and query structured data using SQL: filtering, grouping, joining tables, aggregating, and creating views.
