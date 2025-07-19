## J & J E-Commerce Sales Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Analytics Tools](#analytics-tools)
- [Problem Statement](#problem-statement)
- [Processes](#processes)
- [Brief Statement on the Dataset](#brief-statement-on-the-dataset)
- [Exploratory Data Analysis (KPIs)](#exploratory-data-analysis-kpis)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations).

### Project Overview

This analytical/visualization exercise seeks to extract useful business insights from the sales data of J & J E-Commerce company. Upon analysing the dataset, we identified the key contributors to the company's profits, made recommendations and also identified limitations in the dataset 

### Data Source

ChatGPT - The main data utilized for this analysis/visualization are: __"Product_Analytics, Customer_Data_Enriched and Marketing tables"__.

### Analytics Tools

- Microsoft Power BI
  - [Download Here](https://microsoft.com);
- Power Query on Microsoft Power BI (data cleaning/manipulation/transformation; and
- Figma (for Dashboard's Background Designing).

### Problem Statement

- The data analysed is the one year sales data of J & J Business (the ‘Company’);
- The Company wants to know the key contributors to their profit and possible areas (s) for improvements.

### Processes

1. Data cleaning/tansformation with Power Query interface on Power BI;
2. Data visualizations and dashboarding with Power BI.

### Brief Statement on the Dataset

- The dataset consists of 5 (five) tables;
- The tables utilized for this analytical exercise are 3 – Product_Analytics, Customer_Data and Marketing tables ;
- The profit data (from April 2024 to April 2025) is taken from the Product_Analytics table and not the Financial table.
- The other 2 tables are not considered for this analytical exercise – that is, the Financial and the Operations tables;
- The dataset covers only the USA States.

### Exploratory Data Analysis (KPIs)
Among the key questions answered are:
- Which US state generates the highest profit for the Company;
- In which month did the Company generated the highest profit;
- Which customer generates the highest profit for the Company;
- Which marketing and sales channel generate the highest profit for the Company.

``` sql
SELECT * FROM University
```

### Results/Findings

- Profit as per the customers:
  - Michael Smith generated the highest profit;
  - Female gender generated the highest profit;
  - Age group 35-45 generated the highest profit;
  - Low-Middle income group generated the highest profit;
  - Married customers generated the highest profit;
  - Bachelor’s degree-holding customers generated the highest profit.

- Profit as per products, marketing method and sales channel:
  - Electronics product category generated the highest profit;
  - Sportwear subcategory generated the highest profit;
  - Adidas Hoodie product (under the Sportwear subcategory) generated the       highest profit;
  - Online store/channel generated the highest profit;
  - Billboard campaign type generated the highest profit.

- Profit as per month and states:
  - Kansas (one of the US States) generated the highest profit;
  - Highest profit are generated in the months of July 2024, January 2025 and March 2025. 

### Recommendations

- More focus should be given to the highest profit generating indicators: Kansas state; Billboard campaign type (more profit came from this, even though it has the lowest count when compared to the other 3 campaign types); Online store, Sportwear and Beauty related products, Low-Middle income group, married, bachelor’s degree holders and 35-45 age group;
- The Company should collect data as to reason for its customers churn;
- The absence of churn reasons in the entire 5 tables deprived us the opportunity to know the reason behind each customer’s churn;
- Knowing the reason behind each customer’s churn would allow us know the major churn reason and advise the Company to work duly on the reason.

### Limitations
- Only 3 tables were utilized for the analysis and visualizations:
  - Product_Analytics (PA);
  - Customer_Data_Enriched 1;
  - Marketing
- The Operations and Financial tables were not utilized for the analysis and visualizations.
- The profit column used is that of the PA table – covering only from April 2024 through April 2025 (a year profit).
- The Financial table has a profit column spanning from January 2020 through December 2023 – the Product_Ids that generated the recorded profits here do not bear any correlation with the Product_Ids that generated the profits recorded on the PA table.
- Hence the reason for utilizing the PA, as it is more detailed than the Financials table.
- There are empty cells (missing customer_ids) after Customer_Id 50001 (cell reference: L49003).
- We deleted all those empty cells, to preserve the accuracy of my results/findings.

