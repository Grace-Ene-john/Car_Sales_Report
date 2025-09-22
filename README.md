# Car_Sales_Report Analysis

- [Project Overview](#-project-overview)
- [Dataset Overview](#-dataset-overview)
- [Tools Used](#-tools-used)
- [Key Insights](#-key-insights)
- [Visualization](#-visualizations)
- [SQL Queries](#-sql-queries)
- [Profile](#-profile)

## Project Overview

This project provides insights into car sales data using Excel (Pivot Tables & Charts), SQL, and Power BI.
The dataset contains customer demographics, car specifications, dealer information, and sales performance across regions.
The analysis highlights key trends in customer preferences, sales volume distribution, and regional performance metrics.
SQL was used for querying and cleaning raw data, while Excel supported quick summaries and visualizations.
Power BI brought all insights together in an interactive dashboard, enabling deeper exploration and decision-making.

---

## Dataset Overview
- *Source:* [Car Sales Report – Kaggle](https://www.kaggle.com/datasets/missionjee/car-sales-report)  
- *Size:* 23,906 records  
- *Features:* Customer demographics, car details (company, model, engine, transmission, body style), dealer information, sales price, and region.  

### Sample Records (First 3 Transactions)

| Car_id       | Date     | Customer Name | Gender | Annual Income | Dealer_Name                           | Company  | Model     | Engine                       | Transmission | Color | Price ($) | Dealer_No  | Body Style | Phone   | Dealer_Region |
|--------------|----------|---------------|--------|---------------|----------------------------------------|----------|-----------|------------------------------|--------------|-------|-----------|------------|------------|---------|---------------|
| C_CND_000001 | 1/2/2022 | Geraldine     | Male   | 13,500        | Buddy Storbeck's Diesel Service Inc    | Ford     | Expedition| Double Overhead Camshaft     | Auto         | Black | 26,000    | 06457-3834 | SUV        | 8264678 | Middletown    |
| C_CND_000002 | 1/2/2022 | Gia           | Male   | 1,480,000     | C & M Motors Inc                       | Dodge    | Durango  | Double Overhead Camshaft     | Auto         | Black | 19,000    | 60504-7114 | SUV        | Aurora        |
| C_CND_000003 | 1/2/2022 | Gianna        | Male   | 1,035,000     | Capitol KIA                            | Cadillac | Eldorado | Overhead Camshaft            | Manual       | Red   | 31,500    | 38701-8047 | Passenger  | 7298798 | Greenville    |

---

## Tools Used
- *Excel* → Pivot Tables & Sales Charts  
- *SQL* → Querying and data analysis  
- *GitHub* → Project documentation and portfolio showcase  

---

## Key Insights
- *Total Revenue:* $672M across all sales records.  
- *Top Performing Region:* Austin leads with *$117M in sales*.  
- *Best Selling Body Style:* SUVs dominate with *6,374 units sold*.  
- *Top 5 Locations by Revenue:* Austin, Janesville, Scottsdale, Aurora, and Pasco.  
- *Transmission Split:* Automatic cars contribute *$355M, while manual cars generate **$316M*.  
- *Gender Insights:* Male customers purchased significantly more cars ($527M vs $144M females**).  
- *Top Models:* Models "Huge", "Down", and "Explain" generated the highest sales. 

- *Car Colors:* Black and Pale White cars accounted for nearly *75% of total sales*.
  
---
## Visualization

### Charts
 <img width="1305" height="498" alt="Screenshot 2025-09-22 102341" src="https://github.com/user-attachments/assets/355df76a-fe0d-46ba-a7b9-bb400264a7ea" />


---

## SQL Queries



```sql
---Total revenue by region---
SELECT Dealer_Region, SUM(Price) AS TotalRevenue
FROM car_sales
GROUP BY Dealer_Region
ORDER BY TotalRevenue DESC;
```

```sql
---Most popular car body style---
SELECT BodyStyle, COUNT(*) AS TotalSold
FROM car_sales
GROUP BY BodyStyle
ORDER BY TotalSold DESC;
```

---
## Profile
- **Name:** Grace Ene John
- **Emaill:** enejohn5555@gmail.com
- **LinkedIn:** [Grace-John](https://www.linkedin.com/in/grace-john-b8b622380/)
