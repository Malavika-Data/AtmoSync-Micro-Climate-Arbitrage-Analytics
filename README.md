🥑🍓🍇 AtmoSync — Micro-Climate Arbitrage Analytics

My Team Members : Mameeth C Aparna V Malavika Nair Lucky Aswal 

Infotact Data Analytics Project | Week 1 Report

Real-time IoT sensor analytics to detect in-transit commodity spoilage and identify profitable reroute ("arbitrage") opportunities before goods degrade below quality thresholds.

## 📁 Dataset Description

The AtmoSync dataset contains IoT sensor readings collected from refrigerated shipping containers transporting perishable commodities. The dataset includes environmental conditions, shipment details, quality metrics, and operational information used to monitor cold chain performance.

### Key Attributes

- Container ID
  
- Timestamp
  
- Commodity
  
- Temperature
  
- Humidity
  
- Quality Score
  
- Risk Status
  
- Origin Port
 
- Cooling Unit Status
 
- Arbitrage Gain


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

<img width="927" height="581" alt="Chart Temperature Distribution" src="https://github.com/user-attachments/assets/d5c86988-0e9a-42e7-90d4-40ff2c31db22" />


---

## 2️⃣ Risk Status Distribution

This chart displays the number of containers categorized as Low, Medium, and High risk.

<img width="777" height="527" alt="Chart Risk Status" src="https://github.com/user-attachments/assets/55269110-6d44-4ec1-9ac1-c79ed5eae94c" />


---

## 3️⃣ Top Commodities

This visualization shows the commodities that appear most frequently in the shipment dataset.

<img width="1052" height="647" alt="Chart Top Commodities" src="https://github.com/user-attachments/assets/ca107e84-4da6-42ff-88e7-f79ac91c1992" />


---

## 4️⃣ Temperature vs Humidity

This scatter plot helps analyze the relationship between container temperature and humidity.

<img width="917" height="592" alt="Chart Temp vs Humidity" src="https://github.com/user-attachments/assets/d34fc147-f2db-48bd-953d-84ca77bc0748" />


---

📁 Output

The cleaned dataset is exported as:

cleaned_atmosync_dataset.csv

🚀 How to Run This Project

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



 Week 2 — Dashboard Visualizations & In-Depth Modeling
 <img width="915" height="287" alt="image" src="https://github.com/user-attachments/assets/849c3fcd-b678-47b8-9168-094a9ed7f65d" />

 📊 Key Findings & Visual Insights (Week 2)
 This dashboard was developed using Microsoft Power BI to visualize and analyze the AtmoSync IoT refrigerated container dataset. It provides interactive insights into container performance, risk levels, temperature monitoring, humidity conditions, and commodity distribution.

 Dashboard Features
 
📦 KPI Cards displaying:

Total Containers

Average Temperature

Average Humidity

Average Quality Score

High Risk Containers

Total Arbitrage Gain

📊 Interactive Visualizations:

Risk Status Distribution

Top Commodities

Temperature Trend

Temperature vs Humidity

Quality Score by Commodity

Origin Port Analysis

Cooling Unit Status

🎛 Interactive Slicers:

Commodity

Origin Port

Technologies Used
Microsoft Power BI

DAX (Data Analysis Expressions)

Data Modeling

Interactive Dashboards

Key Insights

Monitored refrigerated container performance using IoT sensor data.

Compared temperature and humidity patterns across shipments.

Identified high-risk containers requiring immediate attention.

Analyzed commodity distribution and quality scores.

Created a dynamic dashboard with interactive filtering for better decision-making.

DAX Measures Used

Total Containers

Average Temperature

Average Humidity

Average Quality Score

Total Arbitrage Gain

Learning Outcome

This project helped me gain practical experience in:

Building interactive Power BI dashboards.

Creating DAX measures for business metrics.

Designing KPI cards and visualizations.

Implementing dynamic filtering using slicers.

Transforming raw IoT data into meaningful business insights.

Dashboard PNG
<img width="1332" height="757" alt="image" src="https://github.com/user-attachments/assets/d15d3c95-f92c-4395-b61c-ea0d5c66b901" />














