# Excel_US_Debt_Tracker_Project

## Project Overview
This project analyzes United States public debt data using **Microsoft Excel**. The objective is to clean, transform, and analyze historical debt records to identify growth trends, seasonal patterns, and projected future debt levels. The analysis leverages Excel features such as pivot tables, charts, and time-series forecasting.

---

## Dataset
An existing dataset was used for this project.

**US Public Debt Dataset**
- Federal-level public debt data.
- Historical records available from **1993 through February 15, 2023** (dataset is not current-day).

### Raw Data Fields
- Record Date.
- Debt Held by the Public.  
- Intragovernmental Holdings.  
- Total Public Debt Outstanding.  

---

## Data Dictionary

| Column | Description |
|------|------------|
| Debt Held by the Public | Portion of U.S. public debt held by individuals, corporations, foreign governments, and entities outside the U.S. government |
| Intragovernmental Holdings | Portion of U.S. public debt held by U.S. government agencies |
| Total Public Debt Outstanding | Total of Debt Held by the Public and Intragovernmental Holdings |

---

## Project Scope
- Data inspection and preparation  
- Data cleaning and transformation in Excel  
- Exploratory data analysis (EDA)  
- Data visualization using charts and pivot tables  
- Time-series forecasting  

---

## Data Cleaning
Data cleaning was performed in Excel and included:
- Removal of empty rows and cells  
- Replacement of null values  
- Transposition and restructuring of the dataset into an analysis-ready format   

---

## Exploratory Data Analysis (EDA) & Findings

### Q1: Yearly Debt Percentage Increase (2016–2023)
This analysis calculates the year-over-year percentage change in **Total Public Debt Outstanding** using the final available record of each year and comparing it with the previous year.

**Methodology**
- Year-end values were used (e.g., 12/30/2022 vs. 12/31/2021)
- Formula used:  
(Current Year - Previous Year) / Previous Year * 100
- Analysis period: 2016–2023  
- Results visualized using a line chart  

**Findings**
- The average annual increase in total public debt between 2016 and 2019 was approximately **5%**
- A significant spike occurred in **2020**, likely driven by pandemic-related fiscal policies
- Debt levels after 2020 remain elevated relative to pre-pandemic trends

---

### Q2: Monthly Debt Increase Patterns
This analysis identifies seasonal trends in total public debt changes.

**Methodology**
- Used *Record Date* and *Total Public Debt Outstanding*
- Created a pivot table with:
- Rows: Month
- Values: Average of Total Public Debt Outstanding

**Findings**
- Highest increases typically occur in **January, February, November, and December**
- Lowest increases are generally observed in **April, May, June, and July**
- These patterns suggest seasonal influences related to fiscal cycles and spending behavior

---

### Q3: Projected Growth of Publicly Held Debt (Through 2030)
This analysis forecasts future levels of **Debt Held by the Public** using historical data.

**Methodology**
- Data aggregated by year  
- Maximum annual values selected  
- Excel `FORECAST.ETS` function applied  
- Forecast extended through **2030**

**Findings**
- Gradual growth observed from 1998 to 2007  
- Accelerated growth from 2008 to 2019  
- Sharp increase between 2020 and 2022, reaching approximately **$25 trillion**  
- Forecast projects continued growth, approaching **$33 trillion by 2030**

---

## Conclusion
This project demonstrates how Excel can be used to clean, analyze, and forecast large financial datasets. The results highlight long-term growth trends in U.S. public debt, seasonal fluctuations, and projected increases in the coming years. Further analysis could incorporate economic indicators such as inflation, interest rates, or government spending to provide additional context.

---
