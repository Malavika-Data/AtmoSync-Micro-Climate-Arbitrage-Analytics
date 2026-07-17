🥑🍓🍇 AtmoSync — Micro-Climate Arbitrage Analytics

My Team Members : Mameeth C Aparna V Malavika Nair Lucky Aswal 

Infotact Data Analytics Project | Week 1 Report

Real-time IoT sensor analytics to detect in-transit commodity spoilage and identify profitable reroute ("arbitrage") opportunities before goods degrade below quality thresholds.


✅Week 1: Data Cleaning & Preprocessing

📌 Project Overview

AtmoSync is an IoT-based analytics project designed to monitor refrigerated shipping containers using sensor data. The objective is to prepare high-quality data for spoilage risk prediction and logistics analysis by performing data cleaning, validation, and exploratory analysis.

🎯 Week 1 Objectives

Import and explore the IoT sensor dataset

Perform data quality assessment

Handle missing values and duplicate records

Convert appropriate columns to correct data types

Standardize text fields

Validate business rules

Generate basic visualizations

Export a cleaned dataset for further analysis

🛠 Technologies Used

Python

Pandas

Matplotlib

Jupyter Notebook

📂 Dataset Features

The dataset contains information related to:

Container Details

Commodity Information

Temperature & Humidity Sensors

Transit Details

Shelf Life

Quality Score

Market Prices

Risk Status

Recommended Actions

📊 Visualizations Included

Temperature Distribution

Risk Status Analysis

Top Commodities

Temperature vs Humidity Scatter Plot

# 📊 Exploratory Data Analysis

## 1️⃣ Temperature Distribution

This histogram illustrates the spread of temperature readings collected from refrigerated containers. Most readings fall within the operational range, while a few higher values may indicate potential spoilage risk.

![Temperature Distribution](images/temperature_distribution.png)

---

## 2️⃣ Risk Status Distribution

This chart displays the number of containers categorized as Low, Medium, and High risk.

![Risk Status](images/risk_status.png)

---

## 3️⃣ Top Commodities

This visualization shows the commodities that appear most frequently in the shipment dataset.

![Top Commodities](images/top_commodities.png)

---

## 4️⃣ Temperature vs Humidity

This scatter plot helps analyze the relationship between container temperature and humidity.

![Temperature vs Humidity](images/temperature_vs_humidity.png)

---

## 5️⃣ Quality Score Distribution

This chart presents how product quality scores are distributed across the dataset.

![Quality Score](images/quality_score_distribution.png)

📁 Output

The cleaned dataset is exported as:

cleaned_atmosync_dataset.csv

🚀 How to Run This Project

# Clone the repo
git clone https://github.com/Mameeth-4015/atmosync-analytics.git
cd atmosync-analytics

# Install dependencies
pip install pandas numpy matplotlib seaborn

# Run the cleaning pipeline
python scripts/clean_data.py

# Open the analysis notebook
jupyter notebook notebooks/week1_eda_and_cleaning.ipynb

📅 Coming in Week 2

 Build baseline visual dashboards (temperature trends, container routes)
 
 Deeper spoilage-curve modeling per commodity
 
 Merge historical commodity pricing trends
 
 Begin Excel/Power BI-style dashboard mockup for stakeholder review
 








