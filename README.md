# Insurance Claims SQL Project

This is a SQL-only data project simulating an insurance database with customer, policy, claim, and agent data. It was created to demonstrate my SQL skills including data generation, table creation, joins, and export to CSV.

## 📊 Project Structure

The database contains 4 main tables:
- `customers`
- `policies`
- `claims`
- `agents`

## ⚙️ Tech Used
- MySQL Workbench
- SQL (Stored Procedures, Joins, Aggregates)

## 📁 Files Included

- `create_tables.sql` – creates the database and tables.
- `populate_data.sql` – generates and inserts 1000 rows per table using stored procedures.
- `join_query_export.sql` – combines tables into one export-ready dataset.
- `insurance_combined_data.csv` – exported result from JOIN query.

## 🔍 Sample Query Output

```sql
SELECT c.full_name, p.policy_type, cl.claim_amount, a.agent_name
FROM customers c
JOIN policies p ON c.customer_id = p.customer_id
JOIN claims cl ON p.policy_id = cl.policy_id
JOIN agents a ON c.region = a.region
LIMIT 10;
