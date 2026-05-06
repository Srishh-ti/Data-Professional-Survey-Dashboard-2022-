# 📊 Data Professional Survey Dashboard (2022) — Power BI

## 🚀 Overview

This project presents an **interactive Power BI dashboard** built to analyze survey responses from data professionals across the globe. The goal was to transform raw, unstructured survey data into a **clean, structured, and insight-driven analytical model**, enabling meaningful exploration of salary trends, career paths, job preferences, and overall satisfaction.

The dashboard follows an **executive-style design approach**, focusing on clarity, usability, and actionable insights.

---

## 🎯 Key Insights

* 💰 **Management roles** command the highest average salaries (~2.5x higher than entry-level roles).
* 🐍 **Python dominates** as the most preferred programming language (~66%).
* 💼 **Compensation is the #1 driver** when considering a new job.
* 🌍 Majority of respondents are from the **United States and India**.
* ⚖️ **Work-life balance and salary satisfaction lag behind management satisfaction**, indicating potential improvement areas.
* 🔄 A significant percentage of professionals are **career switchers**, highlighting the accessibility of data careers.

---

## 🧠 Data Preparation & Transformation

Extensive data cleaning and transformation were performed using **Power Query**:

* Extracted actual values from **“Other (Please Specify)”** responses across multiple columns.
* Converted the **"Current Yearly Salary (in USD)"** column (which contained salary ranges) into a numerical format by calculating the **midpoint of each range**, enabling accurate aggregation and average salary analysis.
* Standardized categorical fields:

  * Role
  * Industry
  * Country
  * Ethnicity
  * Programming Language
  * Job Preferences
* Cleaned inconsistent text formats (case, spacing, duplicates).
* Handled missing/null values appropriately.

### 🔄 Advanced Transformations

* **Unpivoted 6 happiness-related columns (Q6)** into a normalized structure:

  * Created `Dimension` and `Score` columns
  * Simplified long column names into clean labels (e.g., Salary, Work/Life, Learning)
* Created a **custom sort column (Difficulty Order)** to ensure logical sequencing of difficulty levels in visuals
* Structured the dataset for **efficient aggregation and scalable analysis**

---

## 📐 DAX Measures Created

| Measure              | Purpose                                       |
| -------------------- | --------------------------------------------- |
| Total Respondents    | Count of all survey entries                   |
| Avg Salary           | Average of salary midpoint values             |
| Career Switchers %   | % of respondents who switched careers         |
| Found It Difficult % | % who reported difficulty entering data field |
| Avg Happiness Score  | Average across all happiness dimensions       |
| Difficulty Count     | Count used for difficulty distribution        |
| Label                | Static label for stacked bar visualization    |

---

## 📊 Dashboard Features

### 🔹 KPI Summary

* Total Respondents
* Median Salary (K USD)
* Career Switchers %
* Average Happiness Score
* Average Age

### 🔹 Core Visuals

* **Average Salary by Role**
* **Country vs Average Salary**
* **Countries of Respondents**
* **Favorite Programming Language**
* **Education Level Distribution**
* **Difficulty Breaking into Data**
* **What Matters Most in a New Job**
* **Average Happiness Score by Dimension**

### 🔹 Design Approach

* Modern **dark-themed UI** for professional presentation
* Consistent color logic:

  * 🟢 High / Positive
  * 🟠 Medium
  * 🔴 Low / Concern areas
* Clean layout with **card-based structure**
* Focus on **readability and insight clarity**

---

## 🛠 Tools & Technologies

* **Power BI Desktop**
* **Power Query (ETL & Data Cleaning)**
* **DAX (Data Modeling & Measures)**
* **Microsoft Excel (Data Source)**

---

## 📁 Repository Structure

```
data-professional-survey-dashboard/
│
├── dashboard_final.pbix          # Power BI dashboard file
├── dashboard_preview.png        # Dashboard screenshot
├── data/
│   └── raw_dataset.xlsx         # Source dataset                     
└── README.md
```

---

## ▶️ How to Use

1. Download the `.pbix` file
2. Open in **Power BI Desktop**
3. Refresh data (if required)
4. Interact with visuals and filters

---

## 📸 Dashboard Preview

https://github.com/Srishh-ti/Data-Professional-Survey-Dashboard-2022-/dashboard_preview.png

---

## 💡 Project Highlights

* End-to-end **data cleaning → modeling → visualization**
* Real-world handling of **messy survey data**
* Strong focus on **business storytelling**
* Designed to simulate a **production-level analytics dashboard**

---

## 📌 Final Note

This project demonstrates the ability to:

* Transform unstructured data into meaningful insights
* Apply best practices in data modeling and visualization
* Build dashboards that are not just visually appealing, but **decision-oriented**

---

## 🔗 Connect With Me

* LinkedIn: *https://www.linkedin.com/in/srishti-sarswat-475824250/*

---
