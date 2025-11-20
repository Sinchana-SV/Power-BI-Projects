# 🕵🏻‍♀️National Crime in India (2001–2010) – Power BI Dashboard

This repository contains an end-to-end **Power BI analytics project** built on the official **NCRB “Crime in India”** datasets (2001–2010).  

The goal is to convert raw, fragmented Excel tables into an **interactive crime intelligence dashboard** for India – focusing on:

- 📈National crime trends  
- 🤵🏻‍♀️Women & child safety  
- 🥷🏻Kidnapping, murder & rape  
- 💰Economic & financial crime  
- 🚖Police accountability, human-rights violations & housing capacity  

---

## 🔍 Project Overview

👮🏻‍♂️**Problem**

India publishes annual “Crime in India” reports, but most of the data lives in **large, static tables**.  
For a policymaker, student, or citizen it is hard to answer even basic questions like:

- How have different crime categories changed over time?  
- Which **states / UTs** are persistent **hotspots**?  
- Which groups (women, children) are most affected?  
- How effective are the **police and courts** in closing cases?  
- Is there any link between **police capacity (housing)** and **accountability**?

**Objective**

Build a **clean, well-structured Power BI model** that:

1. Integrates multiple NCRB tables (2001–2010) into a **single star schema**  
2. Creates **reliable measures** and **indices** using DAX  
3. Presents insights through **5 thematic dashboard pages**  
4. Is easy to reuse, extend and share (via this GitHub repo)

---

## 🧱 Tech Stack

- **Power BI Desktop**
- **Power Query (M)** for cleaning & shaping data  
- **DAX** for measures, indices & time-intelligence  
- **Star Schema** with dimension tables for `Year`, `Area`, `CrimeType`, etc.

---

## 📂 Data Dictionary
                               
1. **Property_stolen_and_recovered** - Contains state-wise details of property theft incidents, the value stolen, and the value recovered.
2. **Victims_of_rape** - Provides demographic details (age/sex) and counts of rape victims reported across states.
3. **Complaints_against_police** - Captures complaints filed against police personnel, including proven cases and actions taken.
4. **Auto_theft** - Contains data on vehicle theft incidents, types of vehicles stolen, and recovery rates.
5. **Serious_fraud** - Summarizes cases related to major frauds involving financial loss and legal outcomes.
6. **Murder_victim_age_sex** - Provides age and gender details of victims in murder cases reported across states.
7. **CH_not_murder_victim_age_sex** - Covers demographic details of victims of culpable homicide not amounting to murder.
8. **Human_rights_violation_by_police** - Reports cases of human rights violations committed by police, including verified cases and actions.
9. **Police_housing** - Tracks availability, occupancy, and deficits in police residential housing.
10. **Specific_purpose_of_kidnapping_and_abduction** - Categorizes kidnapping incidents based on motive (ransom, marriage, trafficking etc.) with victim counts.
11. **Cases_under_crime_against_women** - Shows statistics of criminal cases filed against women, including type of crime and case outcomes.
12. **Arrests_under_crime_against_women** - Contains data related to arrests, chargesheets, and convictions under crimes against women.

---

## 📊 Dashboard Pages & Key Insights

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/18816ca1-acb0-442b-9523-4d11282de348" />

### 1️⃣ National Crime Dashboard — Executive Summary

**Purpose:**
Give a **single-page national overview** of crime in India (2001–2010).

**Key Features**
**🧮 KPI cards**
- Total Cases (All)
- Total Victims (All)
- Crime Against Women Cases
- Total Custodial Deaths
- Serious Fraud Loss (₹)
- Housing Coverage %

**📈 Trend of Total Cases and Victims by Year**
- Combined bar+line chart shows a **steady rise** in both cases and victims.
- Later years see **victims increasing faster than cases**, indicating growing **impact per case**.

**🗺 National Hotspot Map**
- Composite Severity Index (cases + victims + growth) mapped by **state**.
- Highlights states like **Uttar Pradesh, Maharashtra, Bihar, Rajasthan, West Bengal** as persistent **high-severity hotspots**.

**📋 Area Ranking Table**
- Total Cases, Composite Severity Index, Previous Year Cases, YoY % change and sparklines → quick benchmarking across states.

<img width="960" height="602" alt="image" src="https://github.com/user-attachments/assets/3a4a4545-169b-48fa-9eb5-4e27db79fdcf" />


---

### 2️⃣ Women & Child Safety Overview (2001–2010)

**Purpose:**
Zoom into **Crimes Against Women (CAW)** and child victims, plus backlog and justice outcomes.

**Key Features**

**💟 KPI cards**
- Total Crimes Against Women
- Total Women Victims
- Total Child Victims
- Women’s Safety %

**📈 Trend of Crimes Against Women**
- Shows reported vs convicted vs declared false CAW cases over time.

**🏛 Backlog at Investigation & Trial**
- Investigation Backlog % and Trial Backlog % across states.
- Highlights where justice is slowest for women.

**🧩 CAW Breakdown by Group**
- “Cruelty by husband & relatives” clearly dominates, followed by molestation, kidnapping & rape → **domestic/intimate-partner violence** is a major driver.

**🔻 Justice Pipeline for CAW**
- Reported → Charge-sheeted → Sent for Trial → Trials Completed → Convicted / Acquitted / Withdrawn / Declared False.
- Shows a **large leakage** between reporting and conviction.

**🗺 Women Safety Severity Index by Area**
- Map visual combining CAW load, victim counts and conviction performance into a single severity score.

<img width="642" height="652" alt="image" src="https://github.com/user-attachments/assets/bcac382c-b8a2-4dc9-a8ce-bc298d231c1b" />

---

### 3️⃣ Kidnapping, Murder & Rape — Comparative Analysis

**Purpose:**
Compare three serious violent crimes across **time, victim profile and geography**.

**Key Features**

**🔢 KPIs**
- Total Kidnapping Cases & Victims
- Total Rape Cases & Victims
- Total Murder Victims

**📈 YoY % Change – Kidnapping, Murder, Rape**
- Multi-line chart showing how each crime category is **accelerating or declining**.

**📊 % Share of Rape & Kidnapping Cases by Area**
- Shows which states contribute the **largest slice** of national cases.

**👶🧑‍🦳 Victim Age Distribution by Crime Type**
100% stacked columns:
  - **Kidnapping** → highest **child victim share**
  - **Rape & Murder** → dominated by **adult victims**

**🚺🚹 Female vs Male Victims by Crime Type**
- Rape is overwhelmingly **female-victim**.
- Kidnapping affects **both genders**, while murder is more balanced.

**🧭 Top States by Rape, Kidnapping & Murder Victims**
- Horizontal bars reveal states that are **heavily burdened across multiple serious offences**.

<img width="638" height="651" alt="image" src="https://github.com/user-attachments/assets/a32e2ad3-3ee3-4a5b-8f4f-b88739929865" />

---

### 4️⃣ Economic & Financial Crime Overview

**Purpose:**
Track **serious fraud** losses, value distribution and **auto theft** trends.

**Key Features**
**💰 KPIs**
- Total Serious Fraud Loss
- Total High-Value Fraud
- Fraud Severity Index
- Auto Theft Steals

**🗺 Fraud Loss by Area**
- Map shading by total fraud loss → quickly highlights **financial crime hotspots**.

**🏆 Top 10 Fraud Impact Areas**
- Bar chart of states with the **highest combined loss and high-value fraud**, emphasising need for **stronger financial/cyber-crime units**.

**📊 Fraud Loss Distribution by Value Bucket**
- Long-tail distribution: many low-value cases, but **few extremely large losses dominate the total**.

**🚗 Auto Theft Trend by Vehicle Group**
- Line chart shows **steady rise in vehicle theft**, particularly for motor vehicles, tracking **urbanisation & vehicle growth**.

<img width="478" height="565" alt="image" src="https://github.com/user-attachments/assets/057b1acd-b7b6-4379-b1b9-b899de06f975" />

---
### 5️⃣ Police Accountability, Rights & Capacity

**Purpose:**
Evaluate the **police system itself** – complaints, human-rights violations and housing capacity.

**Key Features**

**📌 KPIs**
- Total Complaints Against Police
- Police Accountability Index
- HRV Total Cases
- HRV Severity Index
- Police Housing Coverage %
- Police Housing Gap %

**📈 Trend of Complaints & HRV Cases**
- Compare how complaints and HRV incidents evolve over time.

**⚖️ Complaint Handling & Outcome Rates**
- Cases Sent for Trial Rate, Departmental / Judicial / Magisterial Enquiry Rates, Police Conviction Rate.
- Reveals **big drop-offs** from complaints to actual convictions.

**🏛 HRV Chargesheet vs Conviction Rate**
- Shows how many HRV cases enter the system vs how many result in punishment.

**🏘 Top 10 States – Police Housing Coverage vs Gap**
- Highlights states with **largest housing deficits**, often overlapping with high-crime / high-complaint states.

**📋 Accountability & Capacity Scorecard**
- Per-state table: complaints, accountability index, HRV metrics, housing coverage & infrastructure index → holistic view of **where both crime and system weaknesses cluster**.

<img width="482" height="482" alt="image" src="https://github.com/user-attachments/assets/bcc10152-1ec3-4f15-a4b7-45c97f4709a1" />

---

### 🔮 Future Enhancements
- Extend to **2011–latest NCRB data** to study recent trends
- Add **population & socio-economic indicators** for crime rates per lakh
- Use **forecasting / clustering** to detect emerging hotspots
- Add **Row Level Security (RLS)** for secure dashboards (e.g., state-specific views)
- Publish to **Power BI Service** or embed in a web / internal portal

