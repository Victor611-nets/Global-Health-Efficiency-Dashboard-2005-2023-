# 🌍 Global Health Efficiency Dashboard (2005–2023)
A Dashboard on Global Health

## 📊 Project Overview

This project analyzes global health outcomes and spending efficiency using data from WHO, World Bank, and Our World in Data (OWID).

The goal is to answer a key question:

> **How efficiently do countries convert health spending into improved health outcomes?**

Using PostgreSQL for data transformation and Tableau for visualization, this dashboard provides a multi-dimensional analysis of life expectancy, health expenditure, and child mortality across countries.

---

## 🧱 Tech Stack

* **SQL (PostgreSQL)** → Data cleaning, transformation, and modeling
* **Tableau Public** → Data visualization & dashboard creation
* **Datasets**:

  * World Health Organization (WHO)
  * World Bank
  * Our World in Data (OWID)

---

## ⚙️ Data Pipeline

### 1. Data Collection

* Imported raw datasets from WHO, World Bank, and OWID

### 2. Data Transformation

* Unpivoted wide-format tables into long format
* Standardized country names across datasets
* Filtered data (2005–2023)
* Created staging tables

### 3. Data Modeling

* Built a final fact table: `fact_global_health`
* Created analytical view: `vw_global_health`
* Added derived metrics:

  * Health expenditure (% of GDP)
  * Life expectancy change (year-over-year)

---

## 📈 Dashboard Features

### 🔹 KPI Overview

* Average Life Expectancy
* Average Health Expenditure (% GDP)
* Average Child Mortality
* Total Countries

### 🔹 Health Efficiency Analysis (Scatter Plot)

* Compares health spending per capita vs life expectancy
* Bubble size represents child mortality
* Color-coded by risk category

### 🔹 Spending Efficiency

* Shows relationship between % GDP spent on health and outcomes
* Includes trend line to highlight correlation

### 🔹 Mortality Impact

* Strong inverse relationship between child mortality and life expectancy

### 🔹 Country Ranking

* Ranks top 20 countries by life expectancy
* Segmented by risk category

---

## 🧠 Key Insights

* Higher health spending does **not always guarantee better outcomes**
* Countries with lower child mortality consistently have higher life expectancy
* Some countries outperform peers despite lower spending (high efficiency)
* High-risk countries cluster around low life expectancy and high mortality

---

## 🎯 Key Skills Demonstrated

* Data Cleaning & Transformation (SQL)
* Data Modeling (Fact tables, Views)
* Window Functions (LAG for trend analysis)
* Data Visualization (Tableau)
* Analytical Thinking & Insight Generation
* Dashboard Design & Storytelling

## 🔗 Live Dashboard

(https://public.tableau.com/authoring/GlobalHealthEfficiencyDashboard20052023/GlobalHealthEfficiencyDashboard20052023#1)

---

## 📌 Future Improvements

* Add efficiency score (custom metric)
* Apply clustering (country segmentation)
* Time-series analysis for trend comparison
* Deploy dashboard with live database connection

---

## 🙌 Author

**Victor Chukwu**
Data Analyst | SQL | Tableau | Data Visualization

---

## ⭐ If you found this useful

Feel free to star the repo and connect!
