# Home_Sales

Overview
This project analyzes home sales data using PySpark and Spark SQL. The steps involve reading the data, creating temporary tables, running SQL queries, caching data, and partitioning Parquet files to optimize query performance. The aim is to answer specific questions about home prices based on different criteria.

Instructions
1. Setup
Rename the Notebook:

Rename the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.
Import Necessary Libraries:

Import the required PySpark SQL functions.
Read Data:

Read the home_sales_revised.csv file into a Spark DataFrame.
Create Temporary Table:

Create a temporary table called home_sales from the DataFrame.
2. SQL Queries
Average Price for Four-Bedroom House per Year:

Write a query to find the average price for a four-bedroom house sold each year. Round off the results to two decimal places.
Average Price for Homes with 3 Bedrooms and 3 Bathrooms:

Write a query to find the average price of homes with three bedrooms and three bathrooms for each year they were built. Round off the results to two decimal places.
Average Price for Specific Criteria:

Write a query to find the average price of homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet for each year they were built. Round off the results to two decimal places.
Average Price per View Rating:

Write a query to find the average price of homes per "view" rating where the average home price is greater than or equal to $350,000. Calculate and display the runtime for this query. Round off the results to two decimal places.
3. Caching and Performance
Cache Temporary Table:

Cache the home_sales temporary table.
Validate Caching:

Check if the home_sales table is cached.
Run Query on Cached Data:

Run the "Average Price per View Rating" query on the cached data. Determine the runtime and compare it to the uncached runtime.
4. Parquet and Partitioning
Partition Data:

Partition the home sales data by the date_built field and save it as Parquet files.
Read Parquet Data:

Read the partitioned Parquet data back into a DataFrame.
Create Temporary Table for Parquet Data:

Create a temporary table for the Parquet data.
Run Query on Parquet Data:

Run the "Average Price per View Rating" query on the Parquet temporary table. Determine the runtime and compare it to the uncached runtime.
5. Cleanup
Uncache Temporary Table:

Uncache the home_sales temporary table.
Verify Uncaching:

Verify that the home_sales table is no longer cached.
6. Final Steps
Download and Upload Notebook:
Download your Home_Sales.ipynb file and upload it to your "Home_Sales" GitHub repository.
Support and Resources
Your instructional team is available to support you during classes and office hours. You also have access to learning assistants and tutors to help you with any topics as needed. Make sure to utilize these resources as you work on this project.

Requirements and Grading
Spark DataFrame Creation :

Create a Spark DataFrame from the dataset.
Temporary Table Creation :

Create a temporary table from the DataFrame.
SQL Queries :

Average price for a four-bedroom house sold each year .
Average price for homes with three bedrooms and three bathrooms for each year they were built.
Average price for homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet for each year they were built .
Average price per view rating with average home price ≥ $350,000, including runtime .
Caching and Validation :

Cache the temporary table and validate caching .
Run the query on cached data and compute runtime .
Parquet and Partitioning :

Partition data by date_built and save as Parquet .
Create a temporary table for Parquet data .
Run the query on Parquet data and compute runtime .
Uncaching and Verification :

Uncache the temporary table and verify uncaching .
