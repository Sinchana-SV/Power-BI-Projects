# 📊 Power BI Projects Portfolio

Welcome to my **Power BI Analytics Portfolio** – a collection of interactive dashboards and end-to-end data projects that showcase my skills in:

- Data cleaning & modelling  
- DAX measure design  
- Story-driven dashboard building  
- Turning raw datasets into **actionable business & policy insights**

---

## 🧭 Projects Overview

| # | Project | Domain | Tech Highlights |
|---|--------|--------|-----------------|
| 1 | [🔍 National Crime in India (2001–2010)](#-1-national-crime-in-india-20012010) | Public Policy / Criminology | Multi-table modelling, composite indices, hotspot analysis, justice pipeline |
| 2 | [🍦 Ice Cream Sales Analysis](#-2-ice-cream-sales-analysis) | Retail / Sales Analytics | Product mix analysis, seasonality, revenue trends, brand-style dashboarding |
| 3 | [🎧 Spotify Streaming Analysis](https://github.com/Sinchana-SV/Power-BI-Projects/tree/main/Spotify%20Streaming) |Digital Media / Streaming Analytics | Converting timestamps to date, hour, and day-of-week, Aggregating minutes, hours, tracks and artists for each visual |
---

## 🧱 Common Tech Stack

- 🟡 **Power BI Desktop**
- 🟢 **Power Query (M)** for data ingestion & cleaning  
- 🔵 **DAX** for measures, time intelligence & indices  
- 🧱 **Star Schema** data modelling (Fact / Dimension tables)  
- 🎨 Focus on **clean UX**, consistent colour themes & intuitive navigation

---

## 🔍 1. National Crime in India (2001–2010)

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/f7fa748c-7eb9-4004-bd02-f52fd443e2d7" />


> **Domain:** Public policy / criminology  
> **Goal:** Build a crime intelligence dashboard from NCRB’s “Crime in India” data (2001–2010).

### 📁 Project Folder

- **Executive Summary Page**
  - National KPIs: **Total Cases**, **Total Victims**, **Crimes Against Women**, **Custodial Deaths**, **Serious Fraud Loss**, **Housing Coverage %**.
  - Yearly trend of cases & victims.
  - **Composite Severity Index** map and hotspot ranking table.

- **Women & Child Safety Page**
  - Crimes against women by category (cruelty by husband/relatives, molestation, rape, etc.).
  - **Justice pipeline** funnel from **Reported → Convicted**.
  - Investigation & trial backlog by state.
  - **Women Safety Severity** map.

- **Kidnapping, Murder & Rape Page**
  - YoY trends for each crime type.
  - **Age & gender vulnerability** comparisons.
  - Top states by rape, kidnapping & murder victims.

- **Economic & Financial Crime Page**
  - Serious fraud losses by state and value bucket.
  - High-value fraud hotspots.
  - Auto theft trends by vehicle type.

- **Police Accountability & Capacity Page**
  - Complaints against police & human-rights violations.
  - Enquiry & conviction rates.
  - Police housing coverage vs gap.
  - Per-state **accountability + capacity scorecard**.

---
##  🔍 2. Ice Cream Sales Analysis

<img width="1167" height="653" alt="image" src="https://github.com/user-attachments/assets/efa2d250-f8af-42be-8ddf-e59c6fc8b663" />


### 🧩 Problem Statement

The ice cream brand has several years of sales stored in **raw spreadsheets**.  
Business teams struggle to answer questions like:

- Which **products, flavours and pack sizes** drive the most **revenue and profit**?
- How do sales change across **months, quarters and years**?
- Which **countries / regions** are the strongest or weakest markets?
- Are there products that are **rising stars** or **declining** and need action (promotion, re-launch, or discontinuation)?

---

### 🗺 Dashboard Highlights

- **Front Page**
  - Full-width image of an **ice cream parlour** for branding and context.
  - Simple navigation buttons to:
    - `Front Page`
    - `Sales Details`
    - `Product Details`
  - Creates a **clean, app-like entry point** to the report.

- **Sales Details Page**
  - KPI cards for **Total Orders**, **Total Quantity Sold**, **Total Revenue**, and **Total Profit / Profit Margin**.
  - **Revenue by SubCategory** (pie/donut) – shows which formats (cones, tubs, popsicles, family packs, etc.) dominate sales.
  - **Revenue by Category** – compares broader segments such as premium vs regular.
  - **Revenue by Year and Product** (column / waterfall) – highlights which products drive year-on-year growth.
  - **Revenue by Category & SubCategory** (stacked columns) – shows the internal mix within each category.
  - **Revenue by Quarter & Month** (line charts) – reveals **seasonality**, with clear summer peaks and off-season dips.
  - **Revenue by Year, Quarter and ProductName** (stacked area / stream graph) – visualises how product contributions shift over time.

- **Product Details Page**
  - Slicers for **Country**, **Year** and **Month_Name** to filter by market and time.
  - **Stream / Stacked Area Chart – Revenue by Year, Quarter and ProductName**
    - Each product (e.g., Alder, Bing, Black Monk, Magnum, Quad, VanHelen, etc.) appears as a distinct coloured band.
    - Makes it easy to spot:
      - **Top-performing products**
      - **Seasonal favourites**
      - Products with **flattening or declining trends**.
  - Used by managers to decide where to:
    - Focus **marketing spend**
    - Launch **new SKUs**
    - Consider **price changes or discontinuation**.

---
## 🎧3. Spotify Streaming Analysis
<img width="697" height="465" alt="image" src="https://github.com/user-attachments/assets/5efb2514-4bbc-4a35-ab80-dca3da6a5071" />


### ✅ Problem Statement

Spotify provides detailed streaming history, but it usually sits in raw JSON/CSV files that are hard to interpret.  
This dashboard was built to answer questions like:

- How many **minutes and hours** have I actually spent listening to Spotify?
- Which **tracks** and **artists** dominate my listening history?
- On which **days of the week** and **times of day** do I listen the most?
- Are there specific **dates** or periods where my listening spikes or drops?

The goal is to turn personal listening data into clear, visual insights about **habits, favourites and time-of-day patterns**.

---

### 📊 Dashboard Highlights

#### 1. Overview Page – *“Spotify Streaming Analysis”*

- **KPI Cards**
  - Total Minutes Played  
  - Total Hours Played  
  - Total Number of Tracks Played  
  - Total Unique Artists  

- **Top 10 Tracks (Bar Chart)**
  - Ranks tracks by **play count** to show the songs on repeat most often.

- **Top 10 Artists by Hours Played (Bar Chart)**
  - Highlights artists with the highest **total listening time**, not just track count.

- **Artist & Song Coverage (Table)**
  - Lists each artist with the number of different songs played.  
  - Useful to see who has both **depth (more tracks)** and **frequency (often played)**.

---

#### 2. Time Patterns Page – *“Listening Behaviour Over Time”*

- **Hours Played by Day of Week (Donut Chart)**
  - Breaks down listening by **Monday–Sunday** to reveal weekday vs weekend habits.

- **Minutes Played by Time of Day (Bar Chart)**
  - Shows total minutes for each **hour (0–23)** to identify morning, afternoon or late-night peaks.

- **Minutes Played by Date (Line Chart)**
  - Time-series of minutes listened per **calendar date**, helping spot binge days and quiet periods.

- **Tracks & Time by Date (Table)**
  - For each date:  
    - Track Count  
    - Total Minutes Played  
    - Total Hours Played  
  - Supports deeper drill-down into specific high-activity days.

---

### 🛠 Tech Notes

- Built in **Power BI** using exported **Spotify Streaming History**.  
- Power Query used for:
  - Converting timestamps to **date, hour, and day-of-week**.
  - Aggregating minutes, hours, tracks and artists for each visual.

---

