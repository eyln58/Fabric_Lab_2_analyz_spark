# Microsoft Fabric - Analyze Data with Apache Spark (Lab 2)

In this lab, I explored how to use Apache Spark in Microsoft Fabric to read, transform, analyze, and visualize structured data. I worked with CSV files stored in a Lakehouse, used PySpark to manipulate data, and generated insights using both SQL queries and Python visualizations.

## 🎯 Objective

- Upload multiple CSV files to a Lakehouse  
- Use Fabric notebooks with PySpark to load and transform data  
- Apply schema definitions and read multiple files with wildcards  
- Perform filtering, aggregation, and grouping operations on a DataFrame  
- Save transformed data in Parquet format (partitioned and unpartitioned)  
- Create and query Delta tables with Spark SQL  
- Visualize results using Fabric’s chart view, matplotlib, and seaborn  

## 🔧 What I Did

### 1. Created a Fabric Workspace and Lakehouse  
I set up a new workspace with Fabric trial capacity and created a Lakehouse to store data files.

### 2. Uploaded CSV Files  
Downloaded a zipped archive of sales order data, extracted it, and uploaded the folder containing CSV files (2019.csv, 2020.csv, 2021.csv) to the Lakehouse.

### 3. Created and Configured a Notebook  
Created a Fabric notebook and added markdown annotations to document my steps. Switched between code and markdown cells to organize the notebook cleanly.

### 4. Loaded Data into a Spark DataFrame  
Used Spark’s read function to load CSV files, first individually and then all at once using a wildcard. Defined a custom schema using Spark SQL types to correctly interpret columns.

### 5. Filtered and Analyzed Data  
Created new DataFrames with selected columns, filtered by product, and counted distinct customers. Grouped sales data by item and year for aggregate analysis.

### 6. Transformed Data  
Added derived columns (Year, Month, FirstName, LastName), reordered columns, and removed unneeded fields to prepare data for downstream analytics.

### 7. Saved Transformed Data  
Saved transformed data in Parquet format for efficient storage. Created partitioned files by Year and Month to support optimized querying.

### 8. Created a Delta Table  
Saved the DataFrame as a managed Delta table named `salesorders`. Queried it using Spark SQL and explored it both programmatically and visually within Fabric.

### 9. Ran SQL Queries  
Used Spark SQL to calculate gross revenue per year directly within notebook cells. Used SQL magic syntax (%%sql) for convenience and clarity.

### 10. Visualized Data  
Used Fabric's chart view to generate bar charts, and then used matplotlib and seaborn to build more customizable charts:  
- Bar and line plots of revenue by year  
- Pie chart showing order distribution  
- Combined subplots for comparison  

## 🧠 What I Learned

- How to structure data engineering workflows in Microsoft Fabric using notebooks and Lakehouses  
- The power of PySpark for reading, transforming, and analyzing data  
- How schema definition impacts data integrity and queryability  
- Benefits of Parquet format and data partitioning in large-scale analytics  
- Delta Lake features within Spark and Fabric for reliable table-based data access  
- Hands-on use of matplotlib and seaborn for professional data visualizations  

## 🔗 Connect with Me

👉 [Follow me on LinkedIn](https://www.linkedin.com/in/eyilan/)
