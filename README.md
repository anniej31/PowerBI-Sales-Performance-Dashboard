# Global Sales Performance Dashboard
---
## Overview
This project is an end-to-end dashboard developed as the capstone project for the Microsoft Power BI Data Analyst Professional Certificate on Coursera. The report simulates a retail analytics project for a home goods company operating across five countries.

## Reports
blah blah
### Sales Overview
Snapshot of overall sales performance, customer loyalty, and product demand.
![Sales Overview](Images/Sales%20Overview.png)
### Profit Overview
blah blah
![Profit Overview](Images/Profit%20Overview.png)
### Key Insights
- a
- b
- c
### Business Recommendations
- a
- b

## Project Workflow
Here is a summary of how the project was built from start to finish.
### Data Sources
The dataset used in this project was provided through the Microsoft Power BI Data Analyst Professional Certificate on Coursera. It is a structured retail sales dataset containing transaction-level records, including order details, customer demographics, geographic information, loyalty status, pricing, cost, and gross profit. The dataset covers the  period from August 2023 to October 2023 and five countries.
After loading the Purchases, Sales, and Countries tables from Excel, a DAX Calendar table was created to support additional calculations. An exchange rate table was also generated using Python to enable currency conversion. A Sales in USD table was also created using DAX to standardize sales values that were originally recorded in multiple currencies.
### Data Cleaning and Transformation
Removed duplicate records and performed data quality checks, including validation of distributions and missing values (none found). Corrected data types where necessary and created custom columns to calculate net profit, cost, gross profit, and total tax.
### Data Modelling
The data model follows a standard star schema structure, with a central Sales fact table connected to multiple dimension tables, including Purchases, Countries, Calendar, Exchange Rates, and Sales in USD.
Relationships were defined as follows:
- Purchases and Sales: 1-to-1 relationship
- Purchases and Calendar: many-to-one relationship
- Sales Table to Sales in USD and Countries Table: many-to-one relationship
- Countries and Exchange Rate tables: 1-to-1 relationship
All relationships were configured with bi-directional (both) cross-filtering to support flexible analysis across the model.
### Aggregations
Custom DAX measures were created to calculate key performance metrics used across both report pages, including;
- **Median Sales**: used instead of the average to reduce the impact of extreme values and provide a more accurate representation of typical sales.
- **Year-to-Date (YTD) Profit**: measures cumulative profitability from the start of the year up to the current date, expressed as a percentage of revenue.
- **Yearly Profit Margin**: calculates overall profitability by comparing net profit to total revenue.
- **Quarterly Profit**: tracks profit performance within each quarter to support short-term trend analysis and comparison across quarters.
### Creating the report
The report was designed in Power BI Desktop with a focus on clarity and consistency. Both pages share the same colour scheme and layout structure. Page navigation buttons were added so users can move between the Sales Overview and Profit Overview pages seamlessly. KPI cards, bar charts, line charts, and pie/donut charts were used depending on what best suited each metric.
### Future Improvements
- Add Month-over-Month (MoM) and Year-over-Year (YoY) measures for deeper trend analysis and performance comparisons over time.
- Implement drill-through pages for products, so that users can explore customer behaviour, sales patterns, and product performance in greater detail.
- Include a table for key sales and profit variales to improve readability and provide additional context alongside visualisations.
  
## Contact
- [My Linkedin](https://www.linkedin.com/in/anniej31/)
- Email: anniejose94@gmail.com
