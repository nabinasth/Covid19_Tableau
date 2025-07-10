# 📊 Report on Visualizing COVID-19 Cases Using Tableau

## 🧾 Introduction

This project focuses on analyzing global COVID-19 trends using the comprehensive **OWID (Our World in Data)** dataset. The dataset includes daily records of confirmed cases, deaths, and vaccination progress, segmented by country and continent.

The **primary objective** is to explore the impact of vaccinations and uncover global patterns using **Tableau dashboards**.

---

## 🗂️ Data Collection and Cleaning

**Tools & Steps:**

- **Data Source:** `owid-covid-data.csv`
- **Language & Libraries:** Python (`pandas`)
- Loaded the dataset and examined its structure
- Removed 19 irrelevant columns to streamline for visualization
- Converted the `date` column to datetime format for time-series analysis
- Created a new column `vaccine_period` to distinguish **Pre-vaccine** and **Post-vaccine** phases based on first non-null vaccination date
- Verified data quality:
  - Checked for missing values
  - Ensured no duplicate records
  - Validated data types
- Exported the cleaned dataset to `.csv` for Tableau use

📐 **Cleaned Dataset Shape:** `166,326 rows × 49 columns`

---

## 📉 Exploratory Data Visualization & Dashboard Overview

**Tool Used:** Tableau

The dashboard includes four main visualizations to explore the pandemic’s progression and vaccination trends globally and by continent:

### 1. **Continent Fully Vaccinated (Bar Chart)**
- Shows total number of fully vaccinated people by continent (Post-vaccine only)
- Europe and North America lead in full vaccination counts

### 2. **People Vaccinated per Year per Continent (Clustered Bar Chart)**
- Annual comparison from 2020 to 2022 across continents
- Asia recorded the highest vaccination peak in 2021

### 3. **Cases, Deaths, and Vaccinations per Continent (Line Chart)**
- Tracks cumulative totals by continent
- Asia shows highest vaccination and death counts, but no clear link between case numbers and vaccine volume

### 4. **Total Cases and Deaths per Year (Line Chart)**
- Global perspective by year
- Significant spike in 2021 for both cases and deaths

---

## 🔍 Key Insights

- Vaccinations ramped up **starting December 2020**, affecting trends in new cases and deaths
- **Europe and North America** lead in full vaccination coverage
- **Asia**, despite the highest volume of vaccinations, still had high case and death counts
- The year **2021** marked the peak for both cases and deaths worldwide

---

## ✅ Conclusion

With Python for data cleaning and **Tableau dashboards** for visualization, this project offers a comprehensive look at the global COVID-19 situation. Comparing pre- and post-vaccine periods provided meaningful insights into the vaccine's impact and regional disparities.

This data-driven approach contributes to a deeper understanding of pandemic dynamics.

---

## 📁 Project Files

- `cleaned_covid_data.csv` – Cleaned dataset used in Tableau
- `covid_analysis.ipynb` – Python notebook for data preprocessing
- `covid_tableau_report.pdf` – Final project report with visualizations
