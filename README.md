# Marketing Campaign Data Analysis
This project uses Power BI to analyse the marketing campaign data and understand the performance, user response and revenue

1)DATA Source:

Data is collected from open CSV files from Kaggle datasource

2) DATA TRANSFORMATION
   
- Renamed the column names for better understanding
- Handled missing values in income column with median income and rounded up the decimal values
- Unpivoted Campaign result, purchase source and product type columns and renamed the resulting columns
- Replaced the values of few categories in Marital_status column into 'Others'


3) CALCULATED COLUMNS

CustomerAge, BirthYear, CustomerTenure

4) CALCULATED TABLE

Date Table with Date Hierarchy 


5) DAX MEASURES
   
- Campaing related: AvgWebVisits, CampaingAcceptanceRate, CampaignSuccess, HighResponders, ResponseRate, ResponsePerUser
- Other: AvgIncome, TotalComplaints, DistinctCustomers, OrderCount, RevenuePerDistinctCustomer, TotwalWebVisits, WebPurchases
- Created Age bins, Income bins and Recency bins

6) Report Structure

Hope page

KPIs:

1. Campaign response rate
2. Number of highly responsive users
3. Average website visits
4. Number of Customers

- This page gives an overview of campaign performance for each campaigns in this series, revenue generation and customer footprints
- A country slicer is available to filter the results for specific locations
- The chart containing revenue information allows to drill through for each product performance and navigates to another page that shows various metrics related to revenue, with filters and slicers synced across the report.
- Home page navigates to a different analysis page using the button that leads to Campaign performance page. This page outlines various customer interaction , website visits grouped by customer age bins, and also compared how likely the web-visits are converted to web purchases 
- This page then navigates to Customer Demographic page that helps understand the userbase and their age distribution

Report Filters:
- age filter is applied on all report pages: age <100
- For Spending analysis, the visual is filtered out for income < 0.2M
- The recently active customers visual considers the result from previous 7 days

