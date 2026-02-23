# task-07
📊 Basic Sales Summary using SQLite and Python
This project demonstrates how to use SQLite with Python to store sales data, run basic SQL queries, and visualize the results using pandas and matplotlib.
- Objective
Create a small SQLite database (sales_data.db)
Store sales information in a single table
Use SQL to calculate:
Total quantity sold per product
Total revenue per product
Display results in the console
Visualize revenue using a bar chart

- Tools & Technologies
Python
SQLite (sqlite3)
Pandas
Matplotlib

  - Project Files
Copy code

├── sales_data.db          # SQLite database
├── sales_summary.py       # Python script
├── sales_chart.png        # Revenue bar chart
└── README.md              # Project documentation

-Database Structure
Table Name: sales
Column
Type
product
TEXT
quantity
INTEGER
price
REAL


- SQL Query Used
SQL
Copy code
SELECT product,
       SUM(quantity) AS total_qty,
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;

Output
Console output showing total quantity and revenue per product
Bar chart visualizing Revenue by Product
Chart saved as sales_chart
