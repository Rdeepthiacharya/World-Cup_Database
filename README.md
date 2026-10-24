# ⚽ World Cup Database

<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-Database-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/SQL-Relational%20Database-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL"/>
  <img src="https://img.shields.io/badge/Bash-Scripting-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash"/>
  <img src="https://img.shields.io/badge/freeCodeCamp-Certification-0A0A23?style=for-the-badge&logo=freecodecamp&logoColor=white" alt="freeCodeCamp"/>
</p>

A PostgreSQL database project built for the **freeCodeCamp Relational Database Certification**.

The database stores knockout-stage match results, including third-place matches, from the FIFA World Cup tournaments held in **2014 and 2018**. It demonstrates relational database design, primary and foreign keys, constraints, data insertion using Bash scripts, and SQL queries for analyzing tournament results.

<br>

## 🗂️ Database Structure

The database contains two related tables: `teams` stores unique teams, while `games` records match results and references participating teams through foreign keys.

| Table | Records | Keys | Main Columns |
|---|---:|---|---|
| `teams` | 24 | **PK:** `team_id` | `name` |
| `games` | 32 | **PK:** `game_id` · **FK:** `winner_id`, `opponent_id` → `teams.team_id` | `year`, `round`, `winner_goals`, `opponent_goals` |

<br>

## 🛠️ Tools & Technologies

* **PostgreSQL** - relational database system
* **SQL** - database query and definition language
* **Bash** - scripting and automation
* **`psql`** - PostgreSQL command-line client
* **`pg_dump`** - PostgreSQL database backup tool

<br>

## 📚 Concepts Demonstrated

* Creating databases and tables
* Primary and foreign keys
* Auto-incrementing IDs using PostgreSQL sequences
* `NOT NULL` and `UNIQUE` constraints
* Inserting data using Bash scripts
* Joining tables using `INNER JOIN`
* Aggregate functions such as `SUM()`, `AVG()`, `MAX()`, and `COUNT()`
* Filtering, sorting, and retrieving distinct records
* Database backup and restoration

<br>

## 📂 Project Files

| File | Description |
|---|---|
| `insert_data.sh` | Bash script to insert unique teams and match records into the database |
| `queries.sh` | Bash script containing SQL queries to analyze World Cup match results |
| `worldcup.sql` | PostgreSQL database dump containing the schema, data, constraints, and relationships |

<br>

<p align="center">
  <strong>⚽ World Cup Database</strong> · Built with PostgreSQL, SQL & Bash
</p>
