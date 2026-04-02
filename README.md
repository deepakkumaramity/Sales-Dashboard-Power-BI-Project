# 🚀 Sales Dashboard (Power BI)

👤 **Created by: Deepak Kumar**

---

## 📊 Project Overview

This project is an **interactive Sales Dashboard** built using Power BI to analyze business performance across **time, regions, and product categories**.

It helps stakeholders make **data-driven decisions** using clear KPIs, trends, and insights.

---

## 🎯 Key Objectives

✔ Track overall business performance
✔ Analyze Month-over-Month (MoM) growth
✔ Monitor Year-to-Date (YTD) revenue
✔ Identify top-performing regions and categories
✔ Provide actionable business insights

---

## 🛠 Tools & Technologies

* 📊 Power BI
* ⚙️ DAX (Data Analysis Expressions)
* 📁 Excel Dataset

---

## 📂 Dataset Details

The dataset contains:

* 📅 Date
* 🌍 Region
* 📦 Category
* 🛒 Product
* 💰 Revenue

---

## ⚡ Step-by-Step Implementation

### 🔹 Step 1: Data Preparation

1. Open Power BI Desktop
2. Click **Get Data → Excel**
3. Load the dataset

---

### 🔹 Step 2: Data Modeling

✔ Ensure Date column is in **Date format**
✔ Create proper relationships (if multiple tables)
✔ Mark Date Table (recommended for time intelligence)

---

### 🔹 Step 3: Create DAX Measures

#### 💰 Total Revenue

```DAX
Total Revenue = SUM(sales_data[Revenue])
```

#### 📉 Previous Month Revenue

```DAX
Previous Month Revenue = 
CALCULATE(
    SUM(sales_data[Revenue]),
    PREVIOUSMONTH(sales_data[Date])
)
```

#### 📈 MoM Growth

```DAX
MoM Growth = 
DIVIDE(
    [Total Revenue] - [Previous Month Revenue],
    [Previous Month Revenue]
)
```

#### 📊 YTD Revenue

```DAX
YTD Revenue = 
TOTALYTD(
    SUM(sales_data[Revenue]),
    sales_data[Date]
)
```

---

### 🔹 Step 4: Dashboard Design<img width="1024" height="1536" alt="Image Apr 2, 2026, 12_46_29 PM" src="https://github.com/user-attachments/assets/7c161b2c-44df-49ae-bea3-b4ef66b594fe" />



#### 📌 KPI Cards

* Total Revenue
* MoM Growth %
* YTD Revenue

#### 📈 Charts

* Line Chart → Revenue Trend
* Bar Chart → Revenue by Region
* Bar Chart → Revenue by Category

#### 🎛 Filters (Slicers)

* Date
* Region
* Category

---

### 🔹 Step 5: Add Business Insights

✔ Revenue increased by 12% MoM
✔ Phone category is the top-performing segment
✔ Delhi region contributes highest revenue
✔ Laptop category shows declining trend

---

## 🧠 Key Insights

📈 Revenue shows consistent growth trend
🌍 Delhi region dominates overall sales
📱 Phone category drives majority of revenue
⚠️ Certain categories need strategic improvement

---

## 💡 Business Impact

This dashboard helps:

✔ Quick decision-making
✔ Identifying growth opportunities
✔ Tracking performance in real-time
✔ Reducing manual reporting efforts

---

## 🖼 Dashboard Preview

👉 (Add your screenshot here: dashboard.png)

---

## 🚀 How to Use

1. Open `.pbix` file in Power BI
2. Use filters to explore data
3. Analyze trends and KPIs
4. Derive insights for business decisions

---

## 🏆 What I Learned

✔ DAX Time Intelligence
✔ Data Visualization Best Practices
✔ Business Storytelling
✔ Dashboard Design Principles

---

## 📢 Connect with Me

If you liked this project, feel free to connect and share feedback!

---

⭐ Don’t forget to star the repository if you found it useful!

---

🔖 **Watermark: Deepak Kumar**
