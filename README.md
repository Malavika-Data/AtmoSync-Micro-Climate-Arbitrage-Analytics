🥑🍓🍇 AtmoSync — Micro-Climate Arbitrage Analytics

My Team Members : Mameeth C Aparna V Malavika Nair Lucky Aswal 

Infotact Data Analytics Project | Week 1 Report

Real-time IoT sensor analytics to detect in-transit commodity spoilage and identify profitable reroute ("arbitrage") opportunities before goods degrade below quality thresholds.


✅ Week 1 — What I Did

#	Task	Status

1	Defined the dataset schema based on the problem statement (sensor + logistics + pricing fields)	✅ Done

2	Generated a realistic 50,000-row synthetic IoT dataset (550 containers × ~91 readings each) using Python	✅ Done

3	Loaded and inspected the dataset in pandas (shape, dtypes, info(), describe())	✅ Done

4	Performed a full 9-step data cleaning process (missing values, duplicates, data types, business-rule validation, outlier flagging)	✅ Done

5	Ran exploratory data analysis (EDA) — risk distribution, correlation analysis, commodity comparison	✅ Done

6	Identified root cause of spoilage (temperature drift from faulty cooling units) using correlation analysis	✅ Done

7	Quantified financial impact of at-risk cargo and rerouting opportunities	✅ Done

8	Documented findings in stakeholder-ready PDF reports	✅ Done

🗂️ Dataset Summary

Property	Value

Total sensor readings	50,000

Containers tracked	550

Commodities covered	Avocado, Banana, Mango, Strawberry, Tomato, Grapes, Blueberry

Reading frequency	Every 30 minutes across a ~50-hour transit journey

Time span	Last 60 days

Data completeness	100% (0 missing values)

Duplicate records	0

Key columns:

Sensor data: temperature_c, humidity_pct, vibration_g

Derived health metrics: quality_score, temp_deviation_c, shelf_life_hours_remaining

Logistics: origin_port, primary_market, secondary_market, distance_primary_km, distance_secondary_km

Financials: primary_price_per_kg_usd, secondary_price_per_kg_usd, arbitrage_gain_usd

Decision output: risk_status (Normal / Watch / At-Risk / Critical), recommended_action

Data Cleaning Process (Python / pandas)
 
All 9 steps were run against the raw dataset before analysis:

<img width="876" height="810" alt="image" src="https://github.com/user-attachments/assets/a2a23268-c0e4-4522-979a-529e33e16c10" />

Cleaning results:

<img width="1071" height="360" alt="image" src="https://github.com/user-attachments/assets/edcdcee0-1df3-49bf-8aab-7428137aac3f" />

Design decision: Outlier sensor readings were flagged, not deleted. In this dataset, an unusual reading is the spoilage signal the business needs — deleting it would hide the exact problem the project exists to detect.

📊 Key Findings (Week 1 EDA)

83% of containers are currently Normal; 13% (74 containers) are At-Risk or Critical and need a routing decision.

Temperature deviation has a strong negative correlation with quality score (r = -0.84) — it's the single biggest driver of spoilage, far more than humidity or vibration.

Faulty cooling units (18.5% of containers) are the root cause of nearly all serious spoilage: average quality score of 40.5 vs. 96.6 for healthy units.

Strawberries, grapes, and blueberries are the most climate-sensitive commodities; tomatoes are the most forgiving.

$538,693 worth of cargo is currently tied up in At-Risk/Critical containers; rerouting the right containers now would capture an estimated $120,533 in additional value.

(Full analysis with charts: see /reports/AtmoSync_Data_Findings_Report.pdf)

🛠️ Tools Used

<img width="702" height="362" alt="image" src="https://github.com/user-attachments/assets/99490d21-2c64-4b2e-a737-247c7b90dc3e" />

📁 Repository Structure

<img width="856" height="462" alt="image" src="https://github.com/user-attachments/assets/3eaea906-02c1-4d7c-ae14-03d07de555ec" />

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
 








