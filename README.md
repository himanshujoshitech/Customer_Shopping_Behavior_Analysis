# 🛍️ Customer Shopping Behavior Analysis – End-to-End Data Analytics Project

![Customer Behavior Dashboard](https://github.com/himanshujoshitech/Customer_Behavior_Shopping_Analysis/blob/main/Power_BI_Dashboard_Screenshot.png)

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

The project follows a structured **end-to-end analytics workflow**, ensuring clarity from problem understanding to final delivery:

1️⃣ **Business Problem Understanding**  
   Define business objectives and identify key analytical questions.

2️⃣ **Data Cleaning & Feature Engineering (Python – Pandas)**  
   Prepare raw data through cleaning, transformation, and feature creation.

3️⃣ **Data Storage & Business Analysis (PostgreSQL – SQL)**  
   Load processed data into PostgreSQL and perform business-driven analysis.

4️⃣ **Interactive Dashboard Creation (Power BI)**  
   Design dashboards to visualize KPIs and uncover trends.

5️⃣ **Insight Generation & Report Writing (PDF)**  
   Summarize findings and convert insights into business recommendations.

6️⃣ **Stakeholder Presentation (Gamma AI)**  
   Communicate insights using AI-powered storytelling for decision-makers.

7️⃣ **Project Publishing & Version Control (GitHub)**  
   Organize and publish the project for collaboration and portfolio use.

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

📁 **File:** [`Python_Code.ipynb`](Python_Code.ipynb)


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
```

### ✅ Insight

Identifies the highest-rated products based on customer feedback.

📁 **SQL Queries File:** `Sql_Code.sql`

---

## 📈 Power BI Dashboard

An interactive **Power BI dashboard** was created to visualize key KPIs and uncover meaningful business patterns.

### 📌 Key Metrics
- **Total Customers:** 3.9K  
- **Average Purchase Amount**  
- **Average Review Rating**

### 📊 Dashboard Insights
- Revenue and sales by product category  
- Subscription vs non-subscription customer comparison  
- Revenue and sales distribution across age groups  
- Impact of discounts and promotions on purchases  

📁 **Dashboard File:** `Power_BI_Dashboard.pbix`

---

## 📑 Report & Presentation

### 📄 Project Report (PDF)
A detailed report covering:
- Analysis methodology  
- Key insights  
- Business recommendations  

### 🤖 Presentation using Gamma AI
A professional, AI-powered presentation created using **Gamma AI**, designed to communicate insights and actionable recommendations effectively to stakeholders.

These deliverables ensure that **technical findings are translated into clear business value**.

---

## 🧠 Key Skills Demonstrated

- End-to-end **data analysis workflow**
- Data cleaning and feature engineering using **Pandas**
- Writing **business-driven SQL queries**
- Database connectivity using **SQLAlchemy**
- Dashboard design and storytelling using **Power BI**
- Professional reporting and **AI-assisted presentation creation**
- Structuring analytics projects for **GitHub portfolios**

---

## ✅ Conclusion

This project demonstrates a **real-world Data Analyst workflow**, combining **Python, SQL, BI tools, and AI** to solve business problems.

It is suitable for:
- 📊 Data Analyst portfolios  
- 💼 Interview discussions  
- 📚 Learning end-to-end analytics projects  

---

## 📬 Connect With Me

If you have feedback, questions, or collaboration ideas, feel free to explore my **GitHub** or connect on **LinkedIn**.

⭐ *If you found this project helpful, consider giving it a star!* ⭐

