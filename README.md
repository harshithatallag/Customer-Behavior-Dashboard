# Customer Shopping Behavior Analysis

## Project Overview

This project analyzes customer shopping behavior using transactional retail data to uncover patterns in customer spending, product performance, discounts, subscriptions, and purchasing frequency. The goal is to transform raw transaction data into actionable insights that support business and marketing decisions.

The workflow uses **SQL for querying and segmentation**, **Python for data cleaning and feature engineering**, and **Power BI for interactive visualization**.

## Business Questions Addressed

The analysis focuses on practical business questions:

* How does revenue differ across customer demographics such as gender and age groups?
* Do subscribed or repeat customers spend more and contribute higher revenue?
* Which products and categories perform best in terms of sales and customer ratings?
* How do discounts and shipping types influence customer spending?
* Which customer segments contribute most to overall revenue?

## Data Overview

The dataset contains approximately 3,900 customer transactions, including:

* Customer demographics: age and gender
* Product and category details
* Purchase amount and review ratings
* Subscription status, discount usage, and shipping type
* Purchase frequency and previous purchase history

This structure reflects real-world retail transaction data commonly used in customer behavior analysis.

## SQL Analysis

SQL was used to perform structured analysis directly on the customer transaction table. Key analyses include:

* Comparing revenue across male and female customers
* Identifying customers who used discounts but still spent above average
* Ranking top products by average review ratings
* Comparing average purchase amount across different shipping types
* Evaluating subscription impact by comparing average spend and total revenue between subscribers and non-subscribers
* Calculating discount usage rates at the product level
* Segmenting customers into new, returning, and loyal groups based on purchase history
* Identifying top-selling products within each category using window functions
* Analyzing repeat buyer behavior and its relationship with subscription status
* Assessing revenue contribution by age group

These queries showcase **aggregation, filtering, subqueries, common table expressions, and window functions**, reflecting real analyst work.

## Python Analysis and Data Preparation

Python was used to clean, enrich, and prepare the data for deeper analysis and visualization. Key steps include:

* Initial data exploration and validation using pandas
* Handling missing review ratings by imputing category-level medians
* Standardizing column names for consistency and downstream usability
* Creating derived features such as age groups using quantile-based binning
* Transforming purchase frequency categories into numeric day-based values for comparison
* Identifying and removing redundant columns to improve data quality
* Loading the cleaned dataset into a SQL database via SQLAlchemy for integration with SQL analysis

These steps mirror **real-world data preparation tasks** expected from an entry-to-mid level data analyst.

## Power BI Dashboard

The dashboard turns SQL metrics and Python features into **interactive business insights**. Each element is designed to highlight meaningful patterns and support decision-making.

### Dashboard Structure

**Top Section – Key Performance Indicators**

* Total customers – overview of customer base
* Average purchase amount – tracks revenue trends
* Average review rating – evaluates overall product satisfaction

**Interactive Filters**

* Subscription status – analyze subscribers vs non-subscribers
* Gender – evaluate spending and product preferences
* Product category – assess category performance
* Shipping type – detect operational or behavioral patterns

**Middle Section – Customer Composition and Product Performance**

* Pie chart of customers by subscription status – visualizes recurring vs new customers
* Bar charts for revenue and sales by category – highlights value-driven vs volume-driven categories

**Bottom Section – Demographics Analysis**

* Revenue and sales by age group – identifies high-value vs high-volume customer segments
* Supports marketing and product strategy decisions

### Purpose and Impact

* Stakeholders can identify high-value customers and profitable products at a glance
* Interactivity allows exploration without additional analysis
* Supports actionable business decisions such as subscription campaigns, discount targeting, and inventory prioritization

## Key Insights

* Customer spending is unevenly distributed; a small segment contributes disproportionately to revenue
* Subscribed and repeat customers generate higher total revenue than non-subscribers
* Certain products and categories consistently outperform others in revenue and ratings
* Discount usage varies by product, indicating opportunities for targeted promotions
* Shipping type and purchase frequency influence average spend
* Age groups reveal differences between high-value and high-volume segments

## Why This Project Matters

This project demonstrates core data analyst competencies:

* Translating business questions into SQL queries
* Cleaning and enriching data using Python
* Applying analytical thinking beyond surface-level exploration
* Communicating insights through dashboards instead of raw tables

It mirrors the **type of work expected in entry-to-mid level data analyst roles**.

## Repository Structure

* `customer_analysis.sql` – SQL queries for segmentation, revenue, and product performance analysis
* `Customer_Shopping_Behavior_Analysis.ipynb` – Python notebook for data cleaning, feature engineering, and exploratory analysis
* `Customer_Behavior_Dashboard.pbix` – interactive Power BI dashboard


