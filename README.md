This project connects Python to a SQLite database, runs SQL queries to get total quantity and revenue by product, and visualizes the revenue using a bar chart. Includes auto-generated sample sales data.

## How to Run
1. Install dependencies:
```bash
pip install pandas matplotlib

## Run the script
python task7_sales_summary.py


##SQL query used
SELECT 
  product,
  SUM(quantity) AS total_qty,
  ROUND(SUM(quantity * price), 2) AS revenue
