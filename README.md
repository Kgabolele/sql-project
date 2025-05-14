# 💼 SQL Portfolio Project: Insurance Company Database

## 📌 Project Objective

This project simulates an insurance company’s database system using pure SQL. The aim is to showcase SQL skills through data creation, manipulation, and analysis without using Power BI or Excel.

---

## 🧱 Database Design

### 1. `customers`
| Column Name | Data Type | Description            |
|-------------|------------|------------------------|
| customer_id | INT        | Unique ID per customer |
| full_name   | VARCHAR    | Full customer name     |
| gender      | CHAR(1)    | 'M' or 'F'             |
| age         | INT        | Age of the customer    |
| region      | VARCHAR    | Province               |

### 2. `policies`
| Column Name | Data Type | Description                 |
|-------------|------------|-----------------------------|
| policy_id   | VARCHAR    | Unique policy number        |
| customer_id | INT        | Linked to `customers` table |
| policy_type | VARCHAR    | Type of policy: Home, Auto, Life |
| start_date  | DATE       | Policy start date           |
| end_date    | DATE       | Policy end date             |
| premium     | DECIMAL    | Premium amount in ZAR       |

### 3. `claims`
| Column Name | Data Type | Description                      |
|-------------|------------|----------------------------------|
| claim_id    | VARCHAR    | Unique claim ID                 |
| policy_id   | VARCHAR    | Linked to `policies` table      |
| claim_date  | DATE       | Date of the claim               |
| claim_amount| DECIMAL    | Amount claimed in ZAR           |
| claim_type  | VARCHAR    | Accident, Death, or Fire        |
| status      | VARCHAR    | Approved, Rejected, or Pending  |

### 4. `agents`
| Column Name | Data Type | Description            |
|-------------|------------|------------------------|
| agent_id    | VARCHAR    | Unique agent ID        |
| agent_name  | VARCHAR    | Full name              |
| region      | VARCHAR    | Province               |
| total_clients| INT       | Number of clients managed |

---

## 🔍 SQL Skills Demonstrated

✅ Data generation using stored procedures  
✅ Data validation and referential integrity  
✅ Complex joins, subqueries, and aggregations  
✅ CASE statements and filtering  
✅ Exploratory data analysis using SQL only  

---

## 📊 Key Analysis Queries

See below for some of the queries I wrote for this project.
