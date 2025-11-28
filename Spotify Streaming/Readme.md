# 🎧 Spotify Streaming Analysis Dashboard
<img width="697" height="465" alt="image" src="https://github.com/user-attachments/assets/bea4d3d0-2995-4928-af4d-d2c41a2a4411" />

## 📝 Problem Statement

I wanted to understand **how, when, and what I listen to on Spotify** – not just a list of songs, but clear answers to questions like:

- How many **minutes and hours** do I actually spend listening to music?
- Which **tracks and artists** dominate my listening history?
- On which **days of the week** and **times of day** do I listen the most?
- Are there specific **dates** when my listening spikes?

This project builds an **interactive dashboard** that turns raw Spotify streaming data into insights about **personal listening behaviour and habits**.

---

## 📊 Project Overview

This repository contains a **Power BI dashboard** that analyses Spotify streaming history and summarises it into key KPIs, charts and tables.

The dashboard is split into two main pages:

1. **Overview – “Spotify Streaming Analysis”**
2. **Time Patterns – “Listening Behaviour Over Time”**

Together, they provide a high-level view of total listening time plus detailed breakdowns by **tracks, artists, day, hour, and date**.

---

## 🧾 Key Features & Metrics

### ✅ Primary KPIs

Displayed as cards on the dashboard:

- **Total Minutes Played** – e.g. `5,558.74` minutes  
- **Total Hours Played** – e.g. `92.65` hours  
- **Total Number of Tracks Played** – e.g. `468` tracks  
- **Total Artists** – e.g. `198` unique artists  

These KPIs give a quick snapshot of overall streaming activity.

---

### 🎵 Page 1 – Spotify Streaming Analysis (Overview)

- **Top 10 Tracks (Bar Chart)**  
  Shows the 10 most played tracks by **play count**, helping identify the songs that are on repeat most often.

- **Top 10 Artists by Hours Played (Bar Chart)**  
  Ranks artists based on **total hours listened**, not just track count, to reveal true favourites.

- **Count of Artists and Their Songs (Table)**  
  A detailed table listing:
  - `artistName`
  - `Track_Count` (number of unique songs played by that artist)  

  Useful to see which artists have both **depth (many tracks)** and **frequency (often played)**.

---

### ⏱️ Page 2 – Listening Behaviour Over Time

- **Hours Played by Day (Donut Chart)**  
  Shows the distribution of total listening hours by **day of the week**  
  (e.g., more listening on weekends vs weekdays).

- **Minutes Played by Time of Day (Bar Chart)**  
  Plots total minutes played by **hour of the day (0–23)** to highlight:
  - Morning, afternoon, or late-night listening peaks.

- **Minutes Played by Date (Line Chart)**  
  A time series view of total minutes per **calendar date**, making it easy to spot:
  - Periods of heavy usage  
  - Breaks or low-activity periods

- **Tracks Played by Date (Table)**  
  Tabular view showing for each date:
  - `Track_Count`
  - `Total_Mins_Played`
  - `Total_Hours_Played`  

  Great for drilling into specific high-activity days.

---

## 🛠 Tech Stack

- 🧠 **Tool:** Power BI Desktop (or any modern BI tool)  
- 🗂 **Data Source:** Spotify Streaming History export (JSON/CSV transformed to tabular format)  
- 🔧 **Transformations:** Power Query for:
  - Converting timestamps to **date**, **hour**, and **day-of-week**
  - Aggregating total minutes, hours, tracks, and artists

---

## ▶️ How to Use This Project

1. **Download / clone** this repository.
2. Open the `.pbix` file (e.g. `Spotify_Streaming_Analysis.pbix`) in **Power BI Desktop**.
3. If needed, update the data source path in **Power Query** to point to your local Spotify export.
4. Refresh the data to see your own streaming behaviour reflected in the dashboard.
5. Explore the visuals using filters, hover tooltips, and cross-highlighting.

---

## 🎯 What This Dashboard Helps You Answer

- Who are my **top artists** and **most-played tracks**?
- How much time do I really spend listening to Spotify?
- Which **days** and **times** do I stream the most?
- Are there **specific periods** where my listening habits change?

---

## 💡 Possible Extensions

- Add **genre-level analysis** (if genre data is available).  
- Include **device type** (mobile, desktop, web) breakdowns.  
- Build a **year-on-year** or **month-on-month** comparison page.  

---

⭐ If you like this project or found it inspiring, feel free to **star** the repo and adapt the dashboard to your own Spotify data!
