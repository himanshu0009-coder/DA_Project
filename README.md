# 🛍️ Customer Shopping Behavior Analysis

<p align="center">
  <img src="https://img.shields.io/badge/Data%20Analytics-Project-blue?style=for-the-badge&logo=databricks&logoColor=white" alt="Data Analytics">
  <img src="https://img.shields.io/badge/Python-Analysis-yellow?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/SQL-MySQL-informational?style=for-the-badge&logo=mysql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
</p>

<p align="center">
  <b>Turning 3,900 Customer Transactions Into Actionable Retail Insights</b>
</p>

<p align="center">
  📊 Python &nbsp;•&nbsp; 🗄️ SQL &nbsp;•&nbsp; 📈 Power BI &nbsp;•&nbsp; 💡 Business Intelligence
</p>

---

## 🧭 Navigation

**[📌 Overview](#-overview)** ·
**[🛠️ Tools](#️-tools--technologies)** ·
**[📂 Dataset](#-dataset)** ·
**[🔄 Workflow](#-project-workflow)** ·
**[🔎 EDA](#-exploratory-data-analysis)** ·
**[🗄️ SQL Analysis](#️-business-questions-sql)** ·
**[📊 Dashboard](#-power-bi-dashboard)** ·
**[💡 Insights](#-key-insights)** ·
**[🎯 Recommendations](#-recommendations)** ·
**[📁 Repository](#-repository-structure)**

---

## 📌 Overview

This project is an **end-to-end customer shopping behavior analysis** built around **3,900 retail transactions**.

The goal was to understand what drives:

* 💰 Revenue
* 🛒 Customer spending
* 🏷️ Discount behavior
* 📦 Product performance
* ⭐ Customer satisfaction
* 🔄 Customer loyalty
* 👥 Subscription behavior

The project follows a complete analytics workflow:

```text
📥 Raw Data
    ↓
🧹 Data Cleaning
    ↓
🔎 Exploratory Data Analysis
    ↓
🗄️ SQL Business Analysis
    ↓
📊 Power BI Dashboard
    ↓
💡 Business Insights
    ↓
🎯 Recommendations
```

### 💡 Headline Finding

> **Average order value remains remarkably stable at approximately $58–$60 across gender, age, subscription status, and discount usage.**

This means revenue differences between customer groups are primarily driven by **customer volume**, rather than significant differences in individual spending.

---

## 🛠️ Tools & Technologies

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">
</p>

| 🔧 Tool         | 🎯 Purpose                                       |
| --------------- | ------------------------------------------------ |
| 🐍 **Python**   | Data cleaning, exploration & feature engineering |
| 🐼 **Pandas**   | Data manipulation & analysis                     |
| 🔢 **NumPy**    | Feature engineering & numerical analysis         |
| 🗄️ **MySQL**   | Business questions & SQL analysis                |
| 📊 **Power BI** | Interactive dashboard & visualization            |

---

## 📂 Dataset

**File:** `customer_shopping_behavior.csv`

### 📊 Dataset Snapshot

| Metric              |        Value |
| ------------------- | -----------: |
| 📋 Records          |    **3,900** |
| 🧩 Fields           |       **18** |
| 💵 Purchase Range   | **$20–$100** |
| ⭐ Missing Ratings   |       **37** |
| 👨 Male Customers   |      **68%** |
| 👩 Female Customers |      **32%** |
| 🏷️ Discount Orders |     **~43%** |
| ⭐ Subscribers       |      **27%** |

### 🧾 Dataset Fields

| Field                      | Description                                  |
| -------------------------- | -------------------------------------------- |
| 🆔 **Customer ID**         | Unique customer identifier                   |
| 👤 **Age / Gender**        | Customer demographic information             |
| 🛍️ **Item Purchased**     | Product purchased                            |
| 🗂️ **Category**           | Clothing, Accessories, Footwear or Outerwear |
| 💵 **Purchase Amount**     | Transaction value in USD                     |
| ⭐ **Review Rating**        | Customer rating                              |
| 🔔 **Subscription Status** | Active subscription status                   |
| 🏷️ **Discount Applied**   | Whether a discount was used                  |
| 🎟️ **Promo Code Used**    | Whether a promotional code was used          |
| 🚚 **Shipping Type**       | Shipping method selected                     |
| 🔄 **Previous Purchases**  | Number of previous orders                    |

---

## 🔄 Project Workflow

### 1️⃣ Data Cleaning & Exploration — Python

The dataset was loaded and profiled using **Pandas** and **NumPy**.

Key activities:

* 🧹 Checked missing values
* 🔍 Investigated data types
* 🔁 Checked duplicate customer IDs
* 📊 Examined distributions
* 📈 Identified trends and patterns
* 🧩 Created an `age_group` feature
* 🚨 Checked for potential outliers

### 2️⃣ Business Analysis — SQL

Ten targeted business questions were answered using:

* `SELECT`
* `GROUP BY`
* `CASE`
* Aggregations
* Subqueries
* Window functions
* Ranking logic

### 3️⃣ Visualization — Power BI

The cleaned dataset and analysis were transformed into an interactive **Customer Behavior Dashboard**.

---

## 🔎 Exploratory Data Analysis

### 📊 Key Findings

* ✅ **3,900 rows × 18 columns**
* ✅ No duplicate customer IDs
* ⚠️ Only **Review Rating** contains missing values
* ⚠️ **37 ratings** are missing — approximately **0.9%**
* 💵 Purchase amount ranges from **$20 to $100**
* 💵 Average purchase amount is **$59.76**
* 👨 **68% Male / 32% Female**
* 👕 Clothing represents **44.5%** of purchases
* 👜 Accessories represent **31.8%**
* 👟 Footwear represents **15.4%**
* 🧥 Outerwear represents **8.3%**
* 🏷️ Approximately **43%** of orders used discounts
* 🔔 Approximately **27%** of customers have an active subscription

### 👥 Customer Age Groups

An `age_group` feature was created to support demographic analysis:

```text
🧑 Young Adult
        ↓
👨 Adult
        ↓
🧔 Middle-aged
        ↓
👴 Senior
```

---

# 🗄️ Business Questions — SQL

The SQL analysis answers **10 key business questions**.

|      # | ❓ Business Question                       | 📌 Key Result                                        |
| -----: | ----------------------------------------- | ---------------------------------------------------- |
| **01** | 👨👩 Revenue: Male vs Female              | Male **$157,890** · Female **$75,191**               |
| **02** | 🏷️ Discount users spending above average | **839 customers** · Avg. **$79.79**                  |
| **03** | ⭐ Top 5 products by review rating         | Gloves, Sandals, Boots, Hat, Skirt                   |
| **04** | 🚚 Standard vs Express purchase value     | Express **$60** · Standard **$58**                   |
| **05** | 🔔 Subscribers vs non-subscribers         | Nearly identical average spend                       |
| **06** | 🏷️ Top 5 products by discount rate       | Hat, Sneakers, Coat, Sweater, Pants                  |
| **07** | 🔄 Customer segmentation                  | Loyal **79.9%** · Returning **18.0%** · New **2.1%** |
| **08** | 🏆 Top products by category               | Top 3 identified for each category                   |
| **09** | 🔔 Repeat buyers & subscription           | Subscribers **91%** · Non-subscribers **88%**        |
| **10** | 👥 Revenue by age group                   | Young Adult leads at **$62,143**                     |

📄 **Full SQL analysis:** `new_customer_shopping_behavior.sql`

---

## 📊 Power BI Dashboard

### 🎛️ Customer Behavior Dashboard

The Power BI dashboard converts the analysis into a single-page interactive business intelligence report.

### 📌 KPI Cards

```text
┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐
│ 👥 CUSTOMERS    │  │ 💵 AVG PURCHASE │  │ ⭐ AVG RATING   │
│                 │  │                 │  │                 │
│    3,900        │  │     $59.76      │  │       3.75      │
└─────────────────┘  └─────────────────┘  └─────────────────┘
```

### 📈 Dashboard Visualizations

* 💰 Revenue by Category
* 🛒 Sales by Category
* 👥 Revenue by Age Group
* 📊 Sales by Age Group
* 🔔 Subscription Status
* 📈 Customer behavior trends

### 🎚️ Interactive Filters

Users can dynamically filter the dashboard by:

`Subscription Status` · `Gender` · `Category` · `Shipping Type`

---

## 💡 Key Insights

### 01 — 💰 Revenue Is a Volume Story

Average order value remains within a narrow **$58–$60 range** across major customer segments.

➡️ Revenue differences are therefore driven more by **customer volume** than by individual spending.

---

### 02 — 🔄 Retention Is Strong

```text
🟢 Loyal Customers      79.9%
🟡 Returning Customers  18.0%
🔵 New Customers         2.1%
```

The business appears to retain customers effectively once they enter the ecosystem.

➡️ **Customer acquisition is the bigger opportunity.**

---

### 03 — 🔔 Subscriptions Drive Engagement

Subscribers and non-subscribers have almost identical average purchase values.

➡️ The subscription program appears more connected to **engagement and retention** than increasing basket size.

---

### 04 — 🏷️ Discounting Needs Better Targeting

Approximately half of discount users still spent above the overall average.

➡️ Discounts may not always be generating incremental spending.

**Opportunity:** Target discounts toward new, inactive, or at-risk customers instead of applying them broadly.

---

### 05 — 👕 Clothing & Accessories Lead

Clothing and Accessories together represent **more than three-quarters of the business**.

➡️ These categories should remain central to merchandising, inventory planning, and promotional strategy.

---

## 🎯 Recommendations

| Priority  | Recommendation                                                     |
| --------- | ------------------------------------------------------------------ |
| 🚀 **01** | Invest more heavily in **customer acquisition**                    |
| 🎯 **02** | Make discounts more **targeted and personalized**                  |
| 🔔 **03** | Re-evaluate subscription benefits using **spend-based incentives** |
| 📦 **04** | Monitor margins on high-discount products                          |
| 👕 **05** | Keep Clothing & Accessories central to merchandising               |
| 📊 **06** | Review the Power BI dashboard regularly to identify changes early  |

---

## 📁 Repository Structure

```text
📦 Customer-Shopping-Behavior-Analysis
│
├── 📄 customer_shopping_behavior.csv
│   └── Raw retail transaction dataset
│
├── 🗄️ new_customer_shopping_behavior.sql
│   └── 10 SQL business questions
│
├── 📊 CB_analysis_dashboard.pbix
│   └── Interactive Power BI dashboard
│
└── 📘 README.md
    └── Project documentation
```

---

## 🧠 What This Project Demonstrates

This project demonstrates my ability to take a dataset from **raw data → analysis → visualization → business recommendation**.

### Core capabilities demonstrated:

`🐍 Python` · `🗄️ SQL` · `📊 Power BI` · `🧹 Data Cleaning` · `🔎 EDA` · `📈 Data Visualization` · `💡 Business Analysis`

---

## 👨‍💻 Author

### **[Himanshu Bhardwaj]**

**Data Analyst**

🐍 Python   |   🗄️ SQL   |   📊 Power BI   |   📈 Excel

---

<p align="center">
  <b>📊 Data → 🔎 Insights → 💡 Decisions</b>
  <br><br>
  <i>Thanks for exploring my project! ⭐</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-Python%20%7C%20SQL%20%7C%20Power%20BI-blue?style=flat-square">
</p>
