# 📊 **DAD Projects: Data Access and Analysis**

Hello there! I'm **Nicholas Wyrwas**, a **Software Engineering Student** with a passion for data and how we can use it to drive decisions and insights. In this repository, I’ve gathered a collection of **datasets** and **SQL queries** that I’ve created or worked with, which I believe can help you simplify the process of **data access and analysis**. Whether you're a student, professional, or a company looking to analyze your data efficiently, you'll find useful resources here.

## 📂 **Datasets Overview**

Throughout my studies and professional experience, I've curated datasets from a variety of industries and domains. These datasets represent real-world data across multiple business functions and use cases. Here are the types of datasets available in this repository:

### **1. Sales Data**
- **Purpose**: Analyze performance, trends, and customer behavior.
- **Contents**: Includes transaction records, product details, customer segments, and sales data over time.
- **Use Cases**: 
  - Identify top-performing products and categories.
  - Measure sales trends over time and across different regions.
  - Analyze customer purchasing patterns to drive marketing strategies.

### **2. Employee Data**
- **Purpose**: Explore employee demographics, salaries, and performance metrics.
- **Contents**: Contains information about employees, including their job titles, departments, salary, tenure, performance evaluations, and promotions.
- **Use Cases**: 
  - Calculate average salaries across departments and regions.
  - Analyze employee turnover rates and retention factors.
  - Assess performance metrics to identify high-potential employees.

### **3. Product Inventory**
- **Purpose**: Track inventory levels, product sales, and supplier details.
- **Contents**: Provides data on product IDs, stock levels, product prices, suppliers, and sales over time.
- **Use Cases**: 
  - Monitor stock levels to ensure inventory is sufficient.
  - Identify best-selling products and track restocking needs.
  - Assess supplier performance and delivery times.

### **4. Customer Feedback**
- **Purpose**: Dive into customer feedback sentiments and satisfaction scores.
- **Contents**: Contains feedback surveys, ratings, customer satisfaction scores, and sentiment analysis data.
- **Use Cases**: 
  - Perform sentiment analysis to gauge customer satisfaction.
  - Identify common issues and areas for improvement based on feedback.
  - Correlate feedback with product or service quality.

## 🔍 **SQL Queries**

To analyze the datasets above and uncover valuable insights, I’ve written various SQL queries. These queries serve different purposes, ranging from basic data retrieval to complex analytics. Here’s a summary of the types of queries available in this repository:

### **1. Basic Data Retrieval**
- Simple SQL queries designed to retrieve specific data from individual tables.
- **Example**: 
  ```sql
  SELECT * FROM sales_data WHERE product_id = 101;

  ```

  ### **2. Aggregated Analysis**
Queries that calculate summary statistics or aggregated values across datasets, such as total sales, average employee salaries, or average customer ratings.

**Example:**
```sql
SELECT product_id, SUM(sales_amount) AS total_sales 
FROM sales_data 
GROUP BY product_id;
```
### **3. Advanced Analytics
- Complex SQL queries used for in-depth analysis such as cohort analysis, trend analysis, or advanced filtering techniques.
- **Example**:
  ```sql

  SELECT customer_id, COUNT(order_id) AS order_count
  FROM orders
  WHERE order_date BETWEEN '2024-01-01' AND '2024-03-31'
  GROUP BY customer_id
  HAVING COUNT(order_id) > 5;

  ```
### **4. Join Operations**
Queries that combine data from multiple tables to perform comprehensive analysis.

**Example:**
```sql
SELECT e.employee_id, e.name, s.salary 
FROM employees e
INNER JOIN salaries s ON e.employee_id = s.employee_id;

```
  ### **5. Trend and Time-Series Analysis**
SQL queries designed to extract insights from data over time, like sales trends, monthly growth, or seasonal variations.

**Example:**
```sql
SELECT MONTH(order_date) AS month, SUM(order_amount) AS total_sales 
FROM orders 
GROUP BY MONTH(order_date)
ORDER BY month;
```
### **🔧 Technologies Used**
These datasets and SQL queries were built with and can be used in various relational databases and platforms:

- **SQL (Structured Query Language)**
- **MySQL / PostgreSQL / SQLite** (Database platforms)
- **Microsoft SQL Server** (For Enterprise-grade solutions)
- **Excel / Google Sheets** (For initial data exploration and analysis)

---

### **🧑‍💻 How to Use the Repository**
To get started with these datasets and SQL queries:

1. **Download the Datasets**: You can find all the data files in the `/datasets` directory.
2. **Set Up Your Database**: Import the datasets into a relational database of your choice (MySQL, PostgreSQL, SQLite).
3. **Run SQL Queries**: Use the provided SQL queries in the `/queries` directory to begin analyzing the data.
4. **Modify Queries**: Feel free to modify the queries to suit your own analysis needs or to dive deeper into the data.

If you need help understanding or modifying the queries, feel free to check out the documentation and comments provided alongside each query. I also encourage you to fork this repository and use the datasets for your own projects.

---

### **💡 Key Takeaways**
- **Data Accessibility**: This repository makes it easy to access and explore a variety of real-world datasets.
- **SQL Skill Development**: If you're learning SQL, this is an excellent resource for practicing and improving your query writing.
- **Business Insights**: The datasets cover important business functions like sales, employee performance, and customer feedback, providing valuable insights that can guide decision-making.

---

### **📬 Contact Me**
Feel free to reach out to me if you have any questions or feedback:

- 📧 **Email**: nick.wyrwas@outlook.com
- 🌐 **LinkedIn**: [Nicholas Wyrwas](https://www.linkedin.com/in/nicholaswyrwas)
- 🛠 **GitHub**: [@nwyrwas](https://github.com/nwyrwas)

