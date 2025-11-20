# 🍦 Ice Cream Sales Analysis – Power BI Dashboard

> A sweet little end-to-end **Power BI** project analysing multi-year **Ice Cream Sales Performance** across products, countries, months and seasons.

---

## 🧩 Problem Statement

The ice cream store chain has several years of transaction data, but it lives in **raw Excel/CSV tables**.  
Managers struggle to answer simple, but important, business questions:

- Which **products and flavours** are driving most of the **revenue and profit**?
- How do **sales behave across months, quarters and seasons**?
- Which **countries / markets** are outperforming others?
- Are there any **underperforming products** that need promotion, repositioning or discontinuation?

**Goal:**  
Turn this raw data into an **interactive Power BI dashboard** that gives decision-makers a clear, visual view of **sales trends, product performance and seasonal patterns**.

---

## 🧁 Project Overview

1️⃣This project builds a **three-page Power BI report** for an Ice Cream brand:

1. **Front Page** – Branded landing page with navigation buttons  
2. **Sales Details** – KPI overview, breakdowns and trend analysis  
3. **Product Details** – Deep dive into product performance over time

---
### 2️⃣ Sales Details – Overall Performance
**Purpose:**
Give management a **one-page view** of how the business is performing overall.

**Key Features**
- **🧮 KPI Cards** (examples)
  - Total Orders
  - Total Quantity Sold
  - Total Revenue
  - Total Profit / Profit Margin
    
- **🥧 Revenue by SubCategory**
  - Pie chart showing contribution of different subcategories (e.g., cones, tubs, popsicles, family packs).
  - Quickly highlights **which formats generate maximum revenue**.

- **🥯 Revenue by Category**
  - Separate chart to compare broader categories (e.g., Dairy, Non-Dairy, Premium).

- **📊 Waterfall / Column: Revenue by Year and Product**
  - Shows how each year and product contributes to **overall revenue growth**.
  - Useful for seeing **which flavours or brands drive year-on-year increases**.

- **Stacked Column: Revenue by Category and SubCategory**
  - Combines category and subcategory to show **mix of sales within each category**.

- **📈 Line Charts: Revenue by Quarter & by Month**
    - Quarter view exposes **seasonality** (Q2/Q3 often higher due to summer).
- Month view highlights **peak summer months** and any off-season spikes due to promotions.

- **🌈 Stacked Area / Stream Graph: Revenue by Year, Quarter and Product**
    - Visualises how each **product’s share of revenue** changes over time.
- Great for identifying **rising stars** and **declining flavours**.

<img width="347" height="526" alt="image" src="https://github.com/user-attachments/assets/96d49228-3b1c-4d45-870c-9b9e89550739" />

---

## 3️⃣ Product Details – Deep Dive

**Purpose**:
Enable product managers to **zoom into product-level performance** and seasonality.

**Key Features**
- 🔍 **Slicers**
  - Country
  - Year
  - Month Name

- **🌊 Stacked Area / Stream Graph – Revenue by Year, Quarter and ProductName**
- Displays each product (e.g., Alder, Bing, Black Monk, Magnum, Quad, VanHelen…) as a **layer over time**.
- Makes it easy to:
  - See **which products dominate each quarter**
  - Identify **new launches gaining share**
  - Spot **products that are flattening or declining**

- 📌 Labels on the area chart show approximate revenue per product per quarter, making it easier for stakeholders to **read values without opening tables.**

<img width="1056" height="512" alt="image" src="https://github.com/user-attachments/assets/307c3620-9d98-4357-aa5c-5fe4c49801c4" />

---

## ❓ Business Questions Answered
This dashboard helps answer questions such as:
- Which **top 5 products** generate the highest revenue and profit?
- How do **sales change by month and quarter?** When is the **peak season?**
- Which **countries** contribute most to total revenue?
- Are **premium flavours** actually driving higher margins?
- Which products show **declining trends** and might need **discounts, re-launch or phase-out**?
- How diversified is revenue across the portfolio? Are we **over-dependent on a few products?**
  
---

## 🛠 Tech Stack

- 🟡 **Power BI Desktop**
- 🟢 **Power Query (M)** – data cleaning & shaping  
- 🔵 **DAX** – calculated measures (Revenue, Profit, % of Total, YoY change, etc.)  
- 🧱 **Star Schema** – fact table for sales and dimension tables for Date, Product, Country, Category, SubCategory

---


