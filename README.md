# Project Overview 

**Project Title:** Retail Sales Analysis

**Level:** Beginner

**Database:** retail_sales

This project aims to showcase fundamental SQL techniques commonly employed by data analysts to explore, clean, and analyze retail sales data. It involves designing and populating a relational database, conducting exploratory data analysis (EDA) to uncover trends and patterns, and leveraging SQL queries to address specific business questions and generate actionable insights.

# Objectives:
**1. Database Setup:** Design and initialize a retail sales database by importing and structuring the provided dataset to enable efficient querying and analysis.

**2. Data Cleaning:** Detect and address data quality issues by identifying and handling missing, null, or inconsistent values to ensure data reliability.

**3. Exploratory Data Analysis (EDA):** Conduct preliminary analysis using SQL to explore data distributions, uncover trends, and gain a foundational understanding of the dataset.

**4.Business Analysis:** Formulate and execute SQL queries to answer key business questions, enabling data-driven decision-making and extracting actionable insights.
# Project Structure:
**1. Database Setup** 
-  **Database Creation:** The project starts by creating a database named retail_sales.
-  **Table Creation:**  A table named retail_sales is created to store the sales data. The table structure includes columns for transaction ID, sale date, sale time, customer ID, gender, age, product category, quantity sold, price per unit, cost of goods sold (COGS), and total sale amount.

 '''sql
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
'''
'''sql
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
'''




