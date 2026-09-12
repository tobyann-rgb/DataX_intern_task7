# Task 7: Basic Sales Summary using SQL in Python

## Project Overview
This project bridges the gap between relational databases and Python programming. The objective is to use SQL inside Python to extract fundamental sales metrics—specifically the total quantity sold and total revenue—and present the findings using console print statements alongside a simple bar chart.

## Tools & Libraries
* **Environment:** Python (via Kaggle Notebooks)
* **Database:** SQLite (built natively into Python, requiring no external server setup)
* **Libraries:** 
  * `sqlite3`: To establish the database connection and execute raw schema commands.
  * `pandas`: To execute the analytical SQL query and store results in a DataFrame.
  * `matplotlib`: To generate the visual bar chart.

## Methodology & Execution
1. **Database Initialization:** Created a local, lightweight SQLite database file named `sales_data.db` containing a single `sales` table.
2. **Data Insertion:** Seeded the table with dummy transaction records including product names, quantities, and unit prices.
3. **SQL Aggregation:** Wrote a SQL query using `SUM()` and `GROUP BY` to calculate the total quantity and gross revenue for each unique product.
4. **Data Extraction & Display:** Used `pandas.read_sql_query()` to pull the aggregated SQL results directly into a Python DataFrame, printing the structured summary to the console.
5. **Visualization:** Leveraged `matplotlib.pyplot` to render a simple bar chart visualizing the revenue distribution across the product lines.

## Repository Deliverables
* `task7_sql_in_python.ipynb` — The executed Kaggle notebook containing the Python script.
* `sales_data.db` — The generated local SQLite database file.
* `sales_chart.png` — The exported bar chart visualization.
* `task7.png` — Screenshot confirming successful execution within the Kaggle environment.
