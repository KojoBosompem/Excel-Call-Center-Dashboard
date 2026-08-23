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
1. What is the **Total Call Count** for all Call Representatives?
2. What is the **Total Call Duration** for all Call Representatives?
3. What is the **Average Call Rating** for each call made?
4. How many **5-Star Calls** were recorded?
5. What is the **Weekly Call Trend**?
6. What is the **Monthly Call Trend**?
7. Who is the **Best-Performing Call Representative** by **Total Call Attended To**, **5-Star Calls Ratings Received**, and **Total Revenue Generated** among others.

## Data Analysis

## Results/Findings

## Recommendations

## Limitations

## References




