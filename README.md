## Customer Shopping Behavior Analytics Dashboard

**Python | SQL | Power BI**

### Overview

End to end data analytics project analyzing retail customer transaction data to uncover customer spending patterns, subscription impact, product performance, and demographic driven revenue trends.

This project demonstrates the ability to translate business questions into KPIs, prepare analytics ready data using Python, perform structured SQL analysis, and deliver executive level insights through Power BI dashboards.

---

### Business Objective

The business required a consolidated analytical view to:

Understand which customer segments contribute most to revenue
Evaluate the impact of subscriptions, discounts, and shipping types on spending
Identify high performing products and categories
Support data driven decisions for marketing, pricing, and customer retention

---

### Key KPIs

All KPIs were calculated in SQL and validated against Power BI visuals.

* Total Customers
* Total Revenue
* Average Purchase Amount
* Average Review Rating
* Revenue by Category
* Revenue by Age Group
* Subscriber vs Non Subscriber Revenue

---

### Tools & Technologies

* Python
* Pandas
* MySQL
* Power BI

---

### Phase 1: Data Preparation and Feature Engineering (Python)

Key preparation steps included:

* Data validation and exploratory analysis
* Handling missing review ratings using category level median imputation
* Standardizing column names for consistency and downstream usability
* Creating derived features such as age groups and numeric purchase frequency
* Removing redundant columns to improve data quality
* Loading cleaned data into SQL databases using SQLAlchemy

This process ensured the dataset was analytics ready for SQL querying and BI reporting.

---

### Phase 2: SQL Analysis

SQL was used to answer business critical questions including:

* Revenue comparison between male and female customers
* Identification of discount users who spent above average
* Top products ranked by average customer review rating
* Comparison of average purchase value across shipping types
* Subscription impact analysis across customer count, average spend, and total revenue
* Product level discount usage rates
* Customer segmentation into new, returning, and loyal groups
* Top selling products within each category using window functions
* Repeat buyer behavior and its relationship with subscription status
* Revenue contribution by age group

This phase demonstrates practical SQL usage including aggregations, subqueries, CTEs, and window functions.

---

### Phase 3: Power BI Dashboard Development

Power BI was used to transform SQL outputs into interactive, decision focused dashboards.

#### Dashboard Capabilities

* KPI cards summarizing customer count, average spend, and satisfaction
* Interactive slicers for subscription status, gender, category, and shipping type
* Revenue and sales breakdown by product category
* Customer distribution by subscription status
* Revenue and sales analysis across age groups

The dashboard enables stakeholders to quickly identify high value customers, profitable categories, and behavioral trends without additional analysis.

---

### Power BI Dashboard Preview

Below is a snapshot of the interactive Power BI dashboard created for this project.

**Dashboard Screenshot**

<img width="1626" height="901" alt="Image" src="https://github.com/user-attachments/assets/eecbc25b-6a02-44f1-b184-b67e03647009" />
The full interactive dashboard is available in the repository as
`Customer_Behavior_Dashboard.pbix`.

---

### Key Insights

* Revenue is concentrated among repeat and subscribed customers
* Subscribed customers generate higher total revenue and higher average spend
* Clothing and Accessories contribute the largest share of revenue
* Discount usage varies significantly by product, indicating opportunities for targeted promotions
* Age groups show clear differences between purchase frequency and revenue contribution

---

### Why This Project Matters

This project reflects real world data analyst work by:

* Translating ambiguous business questions into structured analysis
* Combining Python, SQL, and BI tools in a single workflow
* Validating metrics instead of relying solely on BI calculations
* Communicating insights visually for non technical stakeholders

It demonstrates readiness for entry to mid level data analyst roles.

---

### Repository Structure

```
├── Customer_Shopping_Behavior_Analysis.ipynb
├── customer_analysis.sql
├── Customer_Behavior_Dashboard.pbix
├── customer_shopping_behavior.csv
```

