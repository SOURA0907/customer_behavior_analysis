Customer Shopping Behavior Analysis
📌 Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.

The objective is to identify customer spending patterns, product preferences, customer segments, discount behavior, subscription trends, and revenue patterns to support data-driven business decisions.

The project follows an end-to-end Data Analytics workflow:

Python → EDA & Data Cleaning → SQL → Power BI → Business Report → Presentation

📊 Dataset

The dataset contains:

Rows: 3,900
Columns: 18
Transactions: Customer purchase data
Key Features
Category	Features
Customer Demographics	Age, Gender, Location, Subscription Status
Purchase Details	Item Purchased, Category, Purchase Amount, Season, Size, Color
Shopping Behavior	Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases
Customer Feedback	Review Rating
Delivery	Shipping Type

There were 37 missing values in the Review Rating column.

🛠️ Tools & Technologies
Python
Pandas
NumPy
Matplotlib / Seaborn
SQL
PostgreSQL
MySQL
SQL Server
Power BI
Data visualization
Dashboard development
KPI analysis
Gamma
Business presentation / PPT
Jupyter Notebook
Git & GitHub
🔄 Project Workflow
1. Data Loading

Loaded the dataset into Python using Pandas and performed an initial inspection using:

df.info()
df.describe()
Null-value checks
Data-type checks
Duplicate checks

The initial exploration was used to understand the structure and statistical characteristics of the dataset.

2. Exploratory Data Analysis — EDA

Performed EDA to understand:

Customer demographics
Purchase behavior
Product categories
Revenue patterns
Discount usage
Subscription behavior
Customer reviews
Shipping preferences
3. Data Cleaning

The following preprocessing steps were performed:

Handled missing values
Imputed missing Review Rating values using the median rating for each product category
Standardized column names using snake_case
Checked data consistency
Removed the redundant promo_code_used column
Created additional analytical features
Feature Engineering

Created:

age_group
purchase_frequency_days
customer_segment

Customers were segmented into:

New
Returning
Loyal

based on purchase history.

🗄️ SQL Analysis

The cleaned dataset was loaded into PostgreSQL for structured business analysis. The same SQL analysis can be adapted for MySQL or SQL Server with minor syntax changes.

Business Questions

SQL queries were used to analyze:

Revenue by Gender
High-spending customers who used discounts
Top 5 products by average rating
Standard vs. Express shipping
Subscribers vs. non-subscribers
Products with the highest percentage of discounted purchases
Customer segmentation
Top 3 products within each category
Repeat buyers and subscription behavior
Revenue contribution by age group
Example SQL Skills Demonstrated
SELECT
WHERE
GROUP BY
ORDER BY
HAVING
Aggregate functions
CASE WHEN
Subqueries
CTEs
Window functions
Ranking
Business-oriented data analysis
📈 Power BI Dashboard

An interactive Customer Behavior Dashboard was created in Power BI to present the analysis visually.

5
Dashboard Includes
Total Customers
Average Purchase Amount
Average Review Rating
Subscription Status
Revenue by Category
Sales by Category
Revenue by Age Group
Sales by Age Group
Gender filtering
Category filtering
Shipping Type filtering

The dashboard displays approximately 3.9K customers, an average purchase amount of $59.76, and an average review rating of 3.75, based on the dashboard shown in the project report.

📋 Business Insights & Results

Key findings from the analysis include:

Male customers generated higher total revenue than female customers in the analyzed dataset.
Express shipping had a higher average purchase amount than standard shipping: $60.48 vs. $58.46.
The customer base contained 3,116 Loyal, 701 Returning, and 83 New customers based on the defined segmentation.
The top-rated products included Gloves, Sandals, Boots, Hat, and Skirt.
The age-group analysis showed different revenue contributions across Young Adult, Middle-aged, Adult, and Senior segments.
💡 Business Recommendations

Based on the analysis:

Boost Subscriptions — Promote exclusive benefits for subscribers.
Customer Loyalty Programs — Reward repeat buyers and encourage customer retention.
Review Discount Policy — Balance discount-driven sales with margin control.
Product Positioning — Promote top-rated and best-selling products.
Targeted Marketing — Focus campaigns on high-revenue customer segments and relevant shipping preferences.
📑 Business Report

A detailed report was created to document:

Project objective
Dataset overview
Data cleaning process
EDA
SQL analysis
Business questions
Key findings
Power BI dashboard
Business recommendations

The report provides a complete explanation of the analytical process from raw data to business insights.

🎤 Presentation

A professional project presentation was created using Gamma covering:

Project Overview
Business Problem
Dataset
Data Cleaning
EDA
SQL Analysis
Power BI Dashboard
Key Insights
Business Recommendations
Conclusion
▶️ How to Run
1. Clone the Repository
git clone <your-github-repository-url>
cd customer-shopping-behavior-analysis
2. Install Required Libraries
pip install pandas numpy matplotlib seaborn jupyter
3. Run Python Analysis

Open the Jupyter Notebook:

jupyter notebook

Run the notebook containing:

Data loading
EDA
Data cleaning
Feature engineering
Export of cleaned dataset
4. Setup Database

Create a database in PostgreSQL / MySQL / SQL Server and load the cleaned dataset.

Example PostgreSQL connection:

from sqlalchemy import create_engine

engine = create_engine(
    "postgresql://username:password@localhost:5432/database_name"
)

Then execute the SQL scripts provided in the project.

5. Open Power BI
Open the .pbix file.
Connect to the database or cleaned dataset.
Refresh the data.
Explore the interactive dashboard.
6. View Report & Presentation

The project repository contains the business report and Gamma presentation files/links.

📁 Suggested Project Structure
customer-shopping-behavior-analysis/
│
├── data/
│   ├── raw_data.csv
│   └── cleaned_data.csv
│
├── notebooks/
│   └── customer_behavior_analysis.ipynb
│
├── sql/
│   └── business_queries.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── reports/
│   └── customer_behavior_report.pdf
│
├── presentation/
│   └── customer_behavior_presentation.pdf
│
├── requirements.txt
└── README.md
🎯 Skills Demonstrated

Python | Pandas | NumPy | EDA | Data Cleaning | Feature Engineering | SQL | PostgreSQL | MySQL | SQL Server | Power BI | Data Visualization | Business Analysis | Reporting | Presentation
