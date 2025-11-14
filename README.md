# Task-7 – Basic Sales Summary Using SQLite & Python

This task demonstrates how to pull simple sales analytics from a small SQLite database 
and visualize the results using Python.

## 🔧 Tools Used
- Python
- SQLite (built-in)
- Pandas
- Matplotlib

## 📊 SQL Query Used
```sql
SELECT product, 
       SUM(quantity) AS total_qty,
       SUM(quantity * price) AS total_revenue
FROM sales
GROUP BY product;
