# 📊 Customer Analysis & Churn Trends

## 📌 Project Overview

This project analyzes customer subscription and support data to identify **customer churn patterns, retention trends, revenue at risk, customer behavior, and factors associated with churn**.

The project combines **Python, Pandas, NumPy, SQL/SQLite, Matplotlib, and Seaborn** to perform data cleaning, feature engineering, exploratory data analysis, and visualization.

## 🎯 Objectives

* Analyze customer churn and retention
* Identify churn trends across different subscription plans
* Analyze customer behavior by state and gender
* Calculate revenue-related KPIs
* Identify customers at different churn-risk levels
* Analyze the relationship between support escalations and churn
* Visualize important customer trends and patterns

## 🛠️ Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **SQLite**
* **Jupyter Notebook**

## 🔄 Project Workflow

### 1. Data Extraction

Customer, subscription, and support data were extracted from a SQLite database.

The project works with three main tables:

* `db_customer`
* `db_subscription`
* `db_support`

The customer table contains demographic information, while subscription data contains plan, contract, charges, CLTV and churn information. Support data contains complaints, escalations and CSAT scores.

### 2. Data Cleaning

Performed several data-cleaning operations:

* Renamed columns
* Removed unnecessary columns
* Converted date columns to datetime format
* Standardized gender values
* Handled missing country values
* Removed unnecessary support columns

The customer dataset was reduced to relevant fields including customer ID, name, country, state, gender and date of birth.

### 3. Feature Engineering

Created additional analytical features such as:

* `churn_flag`
* `complaint_count`
* `tenure_days`
* `churn_risk`
* `cancellation_month`

The `churn_flag` identifies whether a customer has cancelled their subscription, while `churn_risk` categorizes customers into **Low, Medium and High** risk based on churn score.

### 4. Data Integration

The customer, subscription and support datasets were merged using `customerid` to create a consolidated analysis dataset containing **21 rows and 21 columns**.

## 📈 Key Analysis

The project calculates several important business KPIs:

* Churn Rate
* Retention Rate
* Churn Rate by Plan
* ARPU (Average Revenue Per User)
* Average Customer Tenure
* Revenue at Risk
* Escalation Rate
* Average Complaints per User
* Escalation vs Churn Correlation

### 🔑 Key Findings

* **Churn Rate:** 28.57%
* **Retention Rate:** 71.43%
* **Average Revenue Per User (ARPU):** approximately 18.85
* **Basic Plan Churn:** 60%
* **Standard Plan Churn:** 22.22%
* **Premium Plan Churn:** 14.29%

The analysis shows that the **Basic plan has the highest churn rate**, while the Premium plan has the lowest among the three plans.

## 📊 Data Visualization

The project includes visualizations for:

* Monthly Churn Trend
* Churn by Plan Type
* Churn by State
* Churn by Gender
* Correlation Heatmap
* Pairplot
* Multi-dimensional comparison using Seaborn Catplot
* Plan-wise customer and revenue analysis

The monthly churn visualization tracks churned customers over cancellation months, while other charts compare churn across plans, states and genders.

## 🧮 SQL Integration

SQLite was also used to demonstrate database operations such as:

* Creating tables
* Inserting records
* Reading data using SQL
* Aggregating data using `GROUP BY`
* Connecting SQL databases with Pandas

An example analysis calculates total budget by country using SQL and loads the result into a Pandas DataFrame.

## 💡 Business Insights

The analysis can help a business:

* Identify high-risk customers
* Focus retention strategies on high-churn plans
* Monitor customer support issues
* Identify revenue that may be lost through churn
* Understand customer segments with different churn behavior
* Improve customer retention and subscription strategies

## 📁 Project Structure

```text
Customer-Analysis-Trends/
│
├── DA_project_2.ipynb
├── customer_churn.db
├── exported_churn_data.csv
├── README.md
└── visualizations/
```

## 🚀 Conclusion

This project demonstrates an end-to-end **customer analytics workflow**, starting from database extraction and data cleaning to feature engineering, KPI analysis, visualization and business insights.

It showcases practical skills in **Python, SQL, Pandas, data visualization, exploratory data analysis and customer churn analytics**.
