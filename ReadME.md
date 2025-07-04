\# Kultra Mega Stores Inventory Analysis



This repository contains the SQL queries and analysis performed for the Kultra Mega Stores (KMS) inventory data from 2009 to 2012. The analysis was conducted to support the Abuja division of KMS, focusing on key business insights to aid strategic decision-making.



\## Table of Contents



\- \[Project Overview](#project-overview)

\- \[Case Scenario I - Questions \& Answers](#case-scenario-i---questions--answers)

&nbsp; - \[Question 1: Product Category with Highest Sales](#question-1-product-category-with-highest-sales)

\- \[How to Use](#how-to-use)

\- \[Contributing](#contributing)

\- \[License](#license)



---



\## Project Overview



Kultra Mega Stores (KMS), headquartered in Lagos, specialises in office supplies and furniture, serving individual consumers, small businesses, and large corporate clients across Lagos, Nigeria. This project focuses on analyzing historical order data (2009-2012) for the Abuja division to derive actionable business intelligence.



---



\## Case Scenario I - Questions \& Answers



This section details the answers and the SQL queries used to solve each question from Case Scenario I.



---



\### Question 1: Product Category with Highest Sales



\*\*Question:\*\* Which product category had the highest sales?



\*\*SQL Query:\*\*



To determine the product category with the highest sales, we aggregate the `sales` for each `product\_category` and then order the results in descending order based on the total sales, limiting the output to the top one.



```sql

SELECT

&nbsp;   product\_category,

&nbsp;   SUM(sales) AS TotalSales

FROM

&nbsp;   public.orders

GROUP BY

&nbsp;   product\_category

ORDER BY

&nbsp;   TotalSales DESC

LIMIT 1;



# Kultra Mega Stores Inventory Analysis



This repository contains the SQL queries and analysis performed for the Kultra Mega Stores (KMS) inventory data from 2009 to 2012. The analysis was conducted to support the Abuja division of KMS, focusing on key business insights to aid strategic decision-making.



\## Table of Contents



\- \[Project Overview](#project-overview)

\- \[Case Scenario I - Questions \& Answers](#case-scenario-i---questions--answers)

&nbsp; - \[Question 1: Product Category with Highest Sales](#question-1-product-category-with-highest-sales)

&nbsp; - \[Question 2: Top 3 and Bottom 3 Regions by Sales](#question-2-top-3-and-bottom-3-regions-by-sales)

\- \[How to Use](#how-to-use)

\- \[Contributing](#contributing)

\- \[License](#license)



---



\## Project Overview



Kultra Mega Stores (KMS), headquartered in Lagos, specialises in office supplies and furniture, serving individual consumers, small businesses, and large corporate clients across Lagos, Nigeria. This project focuses on analyzing historical order data (2009-2012) for the Abuja division to derive actionable business intelligence.



---



\## Case Scenario I - Questions \& Answers



This section details the answers and the SQL queries used to solve each question from Case Scenario I.



---



\### Question 1: Product Category with Highest Sales



\*\*Question:\*\* Which product category had the highest sales?



\*\*SQL Query:\*\*



To determine the product category with the highest sales, we aggregate the `sales` for each `product\_category` and then order the results in descending order based on the total sales, limiting the output to the top one.



```sql

SELECT

&nbsp;   product\_category,

&nbsp;   SUM(sales) AS TotalSales

FROM

&nbsp;   public.orders

GROUP BY

&nbsp;   product\_category

ORDER BY

&nbsp;   TotalSales DESC

LIMIT 1;

