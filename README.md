# 📊 Customer Churn Analysis — OTT Streaming Platform

> An end-to-end data analytics project that combines customer, subscription, and support data to understand churn patterns and identify subscribers who may be at risk of cancellation.

---

## 📌 Project Overview

Customer churn is a major challenge for subscription-based streaming platforms. Since customers can easily switch between competing services, businesses need to understand **why subscribers leave** and identify warning signs before cancellation occurs.

This project analyzes customer, subscription, and customer-support data together to create a connected view of subscriber behavior. The analysis is designed to help stakeholders understand churn-related patterns, investigate customer issues, and support data-driven retention planning.

---

## 🎯 Business Challenge

Streaming platforms such as Netflix, Hotstar, and Prime Video operate in a highly competitive environment. Customers may cancel their subscriptions because of pricing, service experience, plan-related concerns, or unresolved support issues.

The central business challenge is:

> **How can a streaming platform identify subscribers who are more likely to churn and understand the factors associated with cancellation?**

This project addresses the challenge by combining multiple data sources and analyzing customer characteristics, subscription details, churn indicators, and support activity.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Combine customer, subscription, and support data into one connected analytical view.
- Clean and prepare data for analysis and reporting.
- Engineer useful features such as customer tenure, churn indicators, and escalation activity.
- Analyze patterns associated with customer churn.
- Investigate the relationship between customer-support escalations and churn.
- Create clear reports and visualizations for business stakeholders.
- Support data-driven customer-retention planning.

---

## 🗂️ Dataset Description

**Database:** `customer_churn`  
**Number of Customers:** 1,300  
**Source File:** `customer_churn_raw_data.xlsx`

The dataset contains three related tables. Each table is connected through the common field `customerid`.

### 1. `db_customer`

| Column | Description |
|---|---|
| `customerid` | Unique customer identifier |
| `name` | Customer name |
| `country` | Customer country |
| `State` | State or region |
| `gender` | Customer gender |
| `dob` | Date of birth |
| `interests` | Customer interests |
| `pincode` | Postal code |

### 2. `db_subscription`

| Column | Description |
|---|---|
| `customerid` | Unique customer identifier |
| `subscription_start_date` | Date when the subscription began |
| `subscription_type` | Individual, Family, or Business |
| `renewal_date` | Next renewal date |
| `plan_type` | Basic, Standard, Premium, or Enterprise |
| `contract_type` | Month-to-Month, One Year, or Two Year |
| `cancellation_date` | Cancellation date, if applicable |
| `cancellation_reason` | Reason for cancellation, if applicable |
| `monthly_charges` | Monthly subscription charge |
| `cltv` | Customer lifetime value |
| `churn_score` | Churn likelihood score from 0 to 100 |

### 3. `db_support`

| Column | Description |
|---|---|
| `customerid` | Unique customer identifier |
| `complaint_date` | Date when a support ticket was raised |
| `Escalations` | Whether the ticket was escalated |
| `csat_score` | Customer satisfaction score from 1 to 5 |
| `col_1` | Support-ticket category |
| `comment` | Support agent's note |

### Data Relationship

```text
db_customer
     |
     | customerid
     |
db_subscription
     |
     | customerid
     |
db_support
```

The common `customerid` field is used to connect the tables and support integrated analysis.

---

## 🧰 Tools and Technologies

### Programming and Data Analysis

- **Python**
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations and feature preparation
- **Matplotlib** — data visualization
- **sqlalchemy** — database connectivity and SQL-based analysis

### Data Preparation

- Data cleaning
- Missing-value handling
- Data-type standardization
- Feature engineering
- Relational data extraction
- Data validation

### Reporting and Visualization

- **Power BI**
- **DAX measures**
- Interactive dashboards
- KPI reporting
- Business-focused charts and insights

---


## ▶️ How to Run the Project

### Prerequisites

Install the following before running the project:

- Python 3.9 or later
- Jupyter Notebook or JupyterLab
- Git
- Power BI Desktop, if you want to open the dashboard

1. **Clone the Repository**

```bash
   github clone https://github.com/sunnyData554-eng/Churn_Analysis_Project 
   cd Churn_Analysis_Project
```

2. **Create a Virtual Environment**

On Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

On macOS or Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```
3. **Install Required Libraries**

```bash
pip install pandas numpy matplotlib sqlalchemy 
```

4. **Open Churn_Analysis.ipynb notebook**

    This file contains:
      - Data Import
      - Data cleaning
      - Data Integration
      - Feature Engineering
      - Exploratory Data Analysis
 
  
5. **Open the Power BI Dashboard**

      - Open Power BI Desktop.
      - Open the `customer_churn_dashboard.pbix` dashboard file.
      - Confirm that the data source path is correct.
      - Refresh the data if required.
      - Review the report pages, KPIs, charts, and DAX measures.
  
6. **Create Project Report and Presentation**

      - Create project report
      - Build presentation deck using AI Tools


---

## 📊 Expected Project Outcome

The project is designed to produce:

- A connected view of customer, subscription, and support data.
- Clean and analysis-ready data.
- Churn-related analytical features.
- Visualizations showing customer and subscription patterns.
- Analysis of the relationship between support escalations and churn.
- A Power BI dashboard for communicating business metrics.
- A structured basis for customer-retention planning.

---

## 🚀 Future Enhancements

Possible future improvements include:

- Building a machine-learning model to predict churn.
- Comparing multiple classification algorithms.
- Evaluating model performance using suitable metrics.
- Creating automated data pipelines.
- Scheduling dashboard refreshes.
- Adding customer-segmentation analysis.
- Deploying analytics workflows to a cloud environment.

---

## 📜 License

MIT — feel free to fork, star, and use in your portfolio.

## 👨‍💻 About the Author
Hey, I’m Sunny Singh, a Data Analyst.
I break down complex data topics into simple, practical content that actually helps you land a job.


- 💼 LinkedIn: [Sunny Singh](https://www.linkedin.com/in/sunnysingh007/)
- 📧 Email: sunny1290singh@gmail.com
- 💻 GitHub: [sunnysingh-analytics05](https://github.com/sunnysingh-analytics05)
- Let’s connect professionally and grow your data career


**💡 Thanks for checking out the project! Your support means a lot! Feel free to star ⭐ this repo or share it with someone learning Data Analytics.🚀**

