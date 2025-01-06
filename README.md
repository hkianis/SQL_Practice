# SQL Practice

[toc]

## Introduction

This repository documents my SQL learning journey. It contains practical queries and projects categorized into:

- **Basic**: Fundamental SQL queries.
- **Intermediate**: Queries with joins, aggregations, and subqueries.
- **Advanced**: Complex queries using window functions, CTEs, and optimizations.

---

## Prerequisites

To use this repository, you need the following tools and resources installed:

1. **PostgreSQL v17.2**  
   [Download PostgreSQL](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)

2. **Chinook Database (PostgreSQL version) v1.4.5**  
   [Download Chinook_PostgreSql.sql](https://github.com/lerocha/chinook-database/releases/tag/v1.4.5)

---

## Setup Instructions

### Step 1: Install PostgreSQL
1. Download PostgreSQL v17.2 from the [official website](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads).
2. Follow the installation steps, ensuring the **pgAdmin** tool is installed.
3. During setup, set a password for the default `postgres` user. You will use this password to connect to the database.

---

### Step 2: Create the `sql_practice` Database
1. Open **pgAdmin** and log in using the `postgres` user credentials.
2. In the **Object Browser**, right-click on **Databases** → **Create** → **Database**.
3. In the **Database Name** field, enter `sql_practice`.
4. Click **Save**.

---

### Step 3: Prepare the Chinook SQL File
1. Download the Chinook SQL file: [Chinook_PostgreSql.sql](https://github.com/lerocha/chinook-database/releases/tag/v1.4.5).
2. Open the SQL file in a text editor (e.g., Notepad++ or VS Code).
3. Remove the following lines from the file:
   ```sql
   /*******************************************************************************
      Drop database if it exists
   ********************************************************************************/
   DROP DATABASE IF EXISTS chinook;

   /*******************************************************************************
      Create database
   ********************************************************************************/
   CREATE DATABASE chinook;

   \c chinook;
	```
4. Save the modified file.
---

### Step 4: Import the Chinook SQL File into sql_practice
1. Open pgAdmin and connect to your PostgreSQL server.
2. Right-click on the sql_practice database → Query Tool.
3. Open the modified Chinook_PostgreSql.sql file and copy its entire contents.
4. Paste the contents into the Query Tool editor.
5. Click Execute (lightning icon) to run the script.
6. Refresh the database tree in pgAdmin to confirm the Chinook tables were successfully created under the sql_practice database.

---

## Repository Structure

```
SQL_Practice/
├── Basic/
│   ├── select_queries.sql       # Simple SELECT statements and filters
│   ├── filtering_queries.sql    # Queries with WHERE clauses
├── Intermediate/
│   ├── joins.sql                # INNER, LEFT, RIGHT joins
│   ├── aggregations.sql         # GROUP BY, HAVING, and aggregate functions
├── Advanced/
│   ├── indexing.sql             # Queries with indexing and optimizations
│   ├── window_functions.sql     # ROW_NUMBER, RANK, and window functions
README.md
```
---

## Tools Used
* PostgreSQL v17.2
* pgAdmin
* Chinook Database v1.4.5

---

## Notes
* This repository is designed for educational purposes.
* Feel free to fork and use the queries for your own learning.

---

## License
[MIT License](https://github.com/hkianis/SQL_Practice?tab=MIT-1-ov-file)

---