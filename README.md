📊 COVID-19 Data Analysis Project
This project explores and analyzes a global COVID-19 dataset to uncover trends in cases, deaths, and socioeconomic indicators like GDP per capita and Human Development Index (HDI). The dataset was sourced from Our World in Data.

📁 Dataset Overview
Source: Publicly available COVID-19 dataset

Rows: 57,394

Columns: 49

Date Range: December 2019 – November 2020

Main Features: Cases, deaths, GDP per capita, HDI, population, health infrastructure

🛠️ Tools Used
Python (Pandas, NumPy)

Seaborn, Matplotlib for visualization

🔍 Key Steps
1. Data Loading and Exploration
Loaded data with Pandas from a remote CSV file

Explored data dimensions, types, and summary statistics

Checked for missing values and data types

2. Data Cleaning
Removed duplicates

Dropped rows with missing continent data

Filled remaining missing values with 0

Converted date column to datetime format

3. Feature Engineering
Extracted month from date

Created total_deaths_to_total_cases ratio

4. Aggregation and Grouping
Grouped by continent and aggregated max values for:

Total cases

Total deaths

GDP per capita

Human Development Index

5. Visualization
Used histograms and bar plots to analyze:

GDP per capita distribution

Total deaths vs. total cases

Deaths-to-cases ratio by continent

📈 Sample Insights
Europe had the highest human development index (0.953).

Africa had the lowest GDP per capita (~661).

Death-to-case ratios varied by continent, with Oceania showing the highest (~3.3%).

📂 Columns Used in Final Analysis
continent

location

date

total_cases

total_deaths

gdp_per_capita

human_development_index

month (engineered feature)

total_deaths_to_total_cases (engineered feature)

✅ Future Work
Predictive modeling of case growth using time-series methods

Correlation analysis between socioeconomic indicators and COVID impact

Country-specific dashboards

✅ How to Run
Clone this repo or download the .ipynb notebook.

Run it in Jupyter Notebook, VSCode, or Google Colab.

Make sure you have the necessary libraries installed:

pip install pandas seaborn matplotlib

All dataset fetching is handled within the code via direct URL.
