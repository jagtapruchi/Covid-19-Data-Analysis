# 📊 COVID-19 Data Analysis

This project explores COVID-19 data globally, analyzing trends in cases, deaths, and the relationship between the pandemic and socioeconomic indicators like GDP per capita and Human Development Index (HDI).

<br/>

## 📁 Dataset Overview

- **Source**: [Our World in Data](https://github.com/SR1608/Datasets/blob/main/covid-data.csv)  
- **Rows**: 57,394  
- **Columns**: 49  
- **Date Range**: Dec 2019 – Nov 2020  
- **Key Features**: Total cases, deaths, GDP per capita, HDI, population, healthcare infrastructure

<br/>

## 🛠️ Tools & Libraries

- **Python**
  - pandas
  - numpy
  - seaborn
  - matplotlib

<br/>

## 🔍 Workflow Summary

### 1. Data Loading & Exploration
- Loaded CSV from GitHub
- Inspected dimensions, types, missing values, and distributions

### 2. Data Cleaning
- Removed duplicates
- Dropped rows with missing `continent`
- Filled other missing values with `0`
- Converted `date` to datetime format

### 3. Feature Engineering
- Created `month` column from `date`
- Added `total_deaths_to_total_cases` ratio

### 4. Grouping & Aggregation
- Grouped by `continent` to analyze:
  - Total cases
  - Total deaths
  - GDP per capita
  - Human Development Index

### 5. Visualization
- Used seaborn/matplotlib for:
  - Histograms of GDP per capita
  - Bar charts of deaths by continent
  - Ratio comparisons

<br/>

## 📈 Key Insights

- **Europe** had the highest average HDI (0.953)
- **Africa** had the lowest average GDP per capita (~661)
- Highest death-to-case ratio observed in **Oceania (~3.3%)**

<br/>

## 📦 Columns Used

- `continent`
- `location`
- `date`
- `total_cases`
- `total_deaths`
- `gdp_per_capita`
- `human_development_index`
- `month` (engineered)
- `total_deaths_to_total_cases` (engineered)

<br/>

## ▶️ How to Run

1. **Clone the Repository**

```bash
git clone https://github.com/yourusername/covid-analysis.git
cd covid-analysis
