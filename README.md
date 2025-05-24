## Project Overview 

**Project Title**: Retail Sales Analysis

**Level**: Beginner

**Database**: `retail_sales`

This project aims to showcase fundamental SQL techniques commonly employed by data analysts to explore, clean, and analyze retail sales data. It involves designing and populating a relational database, conducting exploratory data analysis (EDA) to uncover trends and patterns, and leveraging SQL queries to address specific business questions and generate actionable insights.

### Objectives:
**1. Database Setup:** Design and initialize a retail sales database by importing and structuring the provided dataset to enable efficient querying and analysis.

**2. Data Cleaning:** Detect and address data quality issues by identifying and handling missing, null, or inconsistent values to ensure data reliability.

**3. Exploratory Data Analysis (EDA):** Conduct preliminary analysis using SQL to explore data distributions, uncover trends, and gain a foundational understanding of the dataset.

**4.Business Analysis:** Formulate and execute SQL queries to answer key business questions, enabling data-driven decision-making and extracting actionable insights.

### Project Structure:
**1. Database Setup** 
-  **Database Creation:** The project starts by creating a database named retail_sales.
-  **Table Creation:**  A table named retail_sales is created to store the sales data. The table structure includes columns for transaction ID, sale date, sale time, customer ID, gender, age, product category, quantity sold, price per unit, cost of goods sold (COGS), and total sale amount.
 
```sql
--create database
create database retail_sales

-- create table 
DROP TABLE IF EXISTS retail_sales;
CREATE TABLE retail_sales(
transaction_id INT PRIMARY KEY,	
sale_date DATE,	 
sale_time TIME,	
customer_id	INT,
gender	VARCHAR(15),
age	INT,
category VARCHAR(15),	
quantity	INT,
price_per_unit FLOAT,	
cogs	FLOAT,
total_sale FLOAT
);
```

### 2. Data Exploration & Cleaning

- **Record Count**: Calculates the total number of rows (records) in the dataset.
- **Customer Count**: Determines how many unique customers are present.
- **Category Count**: Lists all unique product categories and counts them.
- **Null Value Check & Cleaning**: Checks for missing data and removes any rows with null values to ensure data quality..

```sql
-- how many sales we have 
  select count(*) as total_sale from retail_sales
-- How many unique customers we have ?
  select count(distinct customer_id) as total_sale from retail_sales
-- how many distinct category we have ?
  select distinct category from retail_sales

select * from retail_sales
where
      transactions_id is null or sale_date is null or sale_time is null or customer_id is null or 
      gender is null or age is null or  category is null or quantiy is null or price_per_unit is null
      or cogs is null or total_sale is null;

delete from retail_sales 
where
    transactions_id is null or sale_date is null or sale_time is null or customer_id is null or
   gender is null or age is null or category is null or quantiy is null or price_per_unit is null or
   cogs is null or total_sale is null;
```

 ### 3. Data Analysis & Findings
 The following SQL queries were developed to answer specific business questions:

 1. **Write a SQL query to retrieve all columns for sales made on '2022-11-05**:
 2. **Write a SQL query to retrieve all transactions where the category is 'Clothing' and the quantity sold is more than 4 in the month of Nov-2022**:
 3. **Write a SQL query to calculate the total sales (total_sale) for each category.**:
 4. **Write a SQL query to find the average age of customers who purchased items from the 'Beauty' category.**:
 5. **Write a SQL query to find all transactions where the total_sale is greater than 1000.**:
 6. **Write a SQL query to find the total number of transactions (transaction_id) made by each gender in each category.**:
 7. **Write a SQL query to calculate the average sale for each month. Find out best selling month in each year**:
 8. **Write a SQL query to find the top 5 customers based on the highest total sales**:
 9. **Write a SQL query to find the number of unique customers who purchased items from each category.**:
 10. **Write a SQL query to create each shift and number of orders (Example Morning <12, Afternoon Between 12 & 17, Evening >17)**:








