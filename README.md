# 🛍️ Customer Shopping Behavior Analysis – End-to-End Data Analytics Project

![Customer Behavior Dashboard](Screenshot%20(20).png)

---

## 🌟 Overview

The **Customer Shopping Behavior Analysis Project** is a complete **end-to-end data analytics project** built on a real-world retail dataset containing **3,900 customer transactions**.  
The goal of this project is to analyze customer purchasing behavior and derive **actionable business insights** using **Python, SQL, Power BI, and AI-powered presentation tools**.

This project follows the **full data analytics lifecycle** — from raw data cleaning to business insights delivery.

---

## 🎯 Business Objective

A retail company wants to understand **how customers shop**, what influences **purchase decisions**, and how different **customer segments** behave across product categories, subscriptions, discounts, and demographics.

### 🧠 Core Business Question:
> **How can the company leverage customer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?**

---

## 🔄 Project Workflow

![Project Workflow](Screenshot%20(21).png)

1️⃣ **Business Problem Understanding**  
2️⃣ **Data Cleaning & Feature Engineering (Python – Pandas)**  
3️⃣ **Data Storage & Business Analysis (PostgreSQL – SQL)**  
4️⃣ **Interactive Dashboard Creation (Power BI)**  
5️⃣ **Insight Generation & Report Writing (PDF)**  
6️⃣ **Stakeholder Presentation using Gamma AI**  
7️⃣ **Project Publishing & Version Control (GitHub)**  

---

## 🛠️ Tools & Technologies Used

- 🐍 **Python** (Pandas, NumPy)
- 🗄️ **PostgreSQL**
- 🔗 **SQLAlchemy & psycopg2**
- 📊 **Power BI**
- 📄 **PDF Report**
- 🤖 **Gamma AI (Presentation)**
- 🌐 **Git & GitHub**

---

## 📊 Dataset Description

The dataset consists of **3,900 customer purchase records** with demographic, transactional, and behavioral attributes.

| Column Name | Description |
|------------|------------|
| `customer_id` | Unique customer identifier |
| `age` | Customer age |
| `gender` | Gender |
| `category` | Product category |
| `item_purchased` | Product name |
| `purchase_amount` | Purchase value (USD) |
| `review_rating` | Customer review rating |
| `subscription_status` | Subscription status |
| `discount_applied` | Discount applied (Yes/No) |
| `frequency_of_purchases` | Purchase frequency |
| `shipping_type` | Shipping method |

---

## 🧪 Data Preparation & Feature Engineering (Python)

Key steps performed using **Pandas**:

- Handling missing values using **group-wise median imputation**
- Standardizing column names
- Feature engineering:
  - **Age group creation** using quartiles
  - **Purchase frequency conversion** from text to numeric days
- Data consistency checks
- Exporting cleaned data to **PostgreSQL**

📁 **File:** `Python_Code.ipynb`

---

## 🧮 Business Analysis Using SQL (PostgreSQL)

After loading the cleaned dataset into PostgreSQL, multiple **business-focused SQL queries** were executed.

### 🔍 Example: Top 5 Products by Average Review Rating

```sql
SELECT 
    item_purchased,
    ROUND(AVG(review_rating)::numeric, 2) AS average_review_rating
FROM customer
GROUP BY item_purchased
ORDER BY average_review_rating DESC
LIMIT 5;

