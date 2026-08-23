# Call-Center Dashboard

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Preparation And Cleaning](#data-preparation-and-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Analysis](#data-analysis)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)


## Project Overview
This project analyzes 200,000 sales and marketing call center records from January to December 2024. The goal was to evaluate agent performance, call outcomes, product effectiveness, customer abandonment reasons, and operational efficiency.
The dataset contains detailed call-level information including agent details, products discussed (Loans, Internet Package, Electronics, Travel Package, Insurance), call duration, outcome (Success / Failure / Abandoned), customer demographics, income bracket, time of day, follow-up requirements, and reasons for abandoned calls.
A full interactive Dashboard and supporting Analysis sheet were built in Excel to monitor key performance indicators (KPIs) and surface actionable insights for sales and operations leadership.


## Data Sources
The data for this project was sourced from Kaggle. A world-renowned website for all types of free yet real business data for all types of analysis. The primary dataset for this project is the Call Centre Data csv file, which contains columns such as **Call Representative**, **Customer ID**, **Call Duration**, **Date of Call**, **Customer Number**, **Satisfaction Rating**, and other calculated columns.


## Tools Used
- Microsoft Excel (with macros – .xlsm)
    - [Download Microsoft Excel Here](https://microsoft.com)
- Power Query (data cleaning & transformation)
- Pivot Tables & Excel formulas (aggregations, success rates, trends)
- Excel Charts & Dashboard design
- Python (pandas, matplotlib, seaborn) – used to recreate and enhance dashboard visuals for this portfolio

 
## Data Preparation and Cleaning
In this part of the project I performed the following tasks;
1. Loaded 200,000 rows × 19 columns from the raw Call Center Data sheet.
2. Handled missing values systematically:
3. Abandoned calls (≈22.3%) correctly had nulls for Product_Discussed, Agent_Rating, and Call_Duration_Minutes.
4. Reason_Call_Abandoned was null for successful and failed calls (expected).
5. Cleaned inconsistent text values in abandonment reasons (long Wait Time vs Long Wait Time → standardized to lowercase).
6. Created a clean full agent name field from Agent_First_Name + Agent_Last_Name.
7. Converted Date to proper datetime and extracted Month for trend analysis.
8. No major duplicate Call_IDs that affected analysis (IDs appear to be short codes rather than unique identifiers).


## Exploratory Data Analysis (EDA)
This involved exploring the Call Centre Data to find insights into Key Performance Metrics
1. **Call Outcomes:** Success 41.8%, Failure 35.9%, Abandoned 22.3%.
2. **Products:** Loans and Internet Package dominate volume; all products show similar success rates (~53–54%) among non-abandoned calls.
3. **Time of Day:** Afternoon has the highest volume, followed by Morning. Evening is significantly lower.
4. **Customer Profile:** Predominantly Male (≈70%), Middle-income bracket most common, average customer age ≈26 years.
5. **Agent Performance:** 13 agents in the dataset; average rating ≈4.25/5. Ratings are very consistent across Success and Failure outcomes.
6. **Abandonment:** Over 94% of abandoned calls are due to long wait times (after cleaning).
7. **Geographic concentration:** New York, California, North Carolina, Nevada, and Texas account for the largest call volumes.


## Data Analysis
Key analyses performed:
- Success rate by product (excluding abandoned calls)
- Average call duration and agent rating by outcome
- Abandonment reason breakdown
- Call volume and success rate by time of day and income bracket
- Monthly call volume trends throughout 2024
- Follow-up requirement rate (≈70% of all calls)
- Repeat customer rate (≈25%)
- State-level volume and success rate comparison
The Analysis sheet contains supporting calculations, lookup tables, and dynamic formulas that feed the Dashboard.


## Results/Findings
•	Overall success rate is 41.8%. When excluding abandoned calls, success rises to ≈53.8%.
•	Long wait time is by far the dominant reason for abandoned calls (≈94%).
•	Average call duration is slightly higher on successful calls (17.5 min) than failed calls (16.2 min).
•	Agent ratings are high and consistent (mean ≈4.25/5) with little difference between successful and failed calls.
•	Follow-up is required on roughly 70% of calls regardless of outcome.
•	Call volume is highest in the Afternoon; success rates are nearly identical across Morning, Afternoon, and Evening.
•	New York has both the highest volume and a relatively strong success rate.


## Recommendations
1.	Reduce wait times – This is the single biggest opportunity. Addressing long wait times could significantly lower the 22.3% abandonment rate.
2.	Investigate staffing levels during peak Afternoon hours.
3.	Review the high follow-up rate (70%) – determine whether processes can be improved to resolve more issues on the first call.
4.	Focus coaching and quality monitoring on the small number of agents (only 13 in the dataset) rather than broad training.
5.	Loans and Internet Package are the highest-volume products with solid success rates – consider prioritizing agent capacity and scripts for these products.
6.	Monitor state-level performance (especially high-volume states) for localized process or training improvements.


## Limitations
•	No customer satisfaction score (CSAT/NPS) beyond the agent rating.
•	No information on call queue time or exact wait duration before abandonment.
•	Agent identifiers are limited (only 13 unique agents), which may not represent a full-scale call center.


## References
•	Source data: Sales and Marketing Call Center.xlsm (Call Center Data, Analysis, and Dashboard sheets)
•	Analysis performed in Microsoft Excel and Python (pandas + matplotlib)



