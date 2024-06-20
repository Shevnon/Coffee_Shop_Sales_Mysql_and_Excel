# Coffee_Shop_Sales_Mysql_and_Excel
An Analysis of a Coffee Shop Sales on different Product Types, Product Category and Store Location over Time

# INTRODUCTION
Coffee  arguably has the highest sales in today's world market for hot drinks.
Analyzing sales data within the coffee industry can offer valuable insights into market trends,customer behaviour and product performance that drive informed
decision-making.
   In this Analysis,I leverage the power of **MYSQL** and **POWER** **BI** to examine Coffee Shop Sales at an hourly,daily,monthly and yearly basis aiming to identify trends and patterns that can inform
business strategies and optimize performance.

# TOOLS UTILIZED
![POWER BI](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Excel/assets/161952555/73010a48-ae97-44ff-9093-824246e56015) 

POWER BI

![mysql-icon](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Excel/assets/161952555/176dee9c-70b3-4e26-8ea5-d023b06791e7)

MYSQL

# SKILLS DEMONSTRATED
* Data cleaning
* Data Analysis Expression(DAX)
* Tooltips
* Data Visulisation and Dashboard creation
* Conditional and custom number format
*  Filters


# METHODOLOGY

## 1. Data Collection and Storage (MYSQL)
* **Data** **Source:** The Primary data set used for the Analysis was gotten from [here](https://drive.google.com/drive/folders/14sSwndELBWmfsBZc5E3dnc4VrgOCemcz)
* **Data** **Extraction:** Data was in xlsx format, so I  first loaded the data using excel then converted to csv format.

  ![image](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Excel/assets/161952555/7afd025b-6886-4a0e-bd92-424cf54661a2)
  
  Data in Excel(xlsx)

![image](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Excel/assets/161952555/72b434e7-c7de-4851-9104-e7520b1188ca)

   Data after being converted to csv

  The next step was to open MySQL workbench,connected to a Local Host, then using a query(create database coffee_shop_sales_db),i created a database and
imported the coffee shop sales table into the database.

* **Data Schema:** The Database contains a single table which contains the following column; transaction_id, transaction_date,transaction_time,transaction_qty,store_id,
store_location,product_id,unit_price,product_category,product_type.

* **Data Integrety:**
 **i. Data Validation Before Import**
* Data format check
* Field Length Validation
* Data integrity rules
* duplicate detection.



 ## 2. Data Cleaning and Preparation (MySQL)
* **Remove Special Characters:** Strip out or normalize special characters that could cause issues.
* **Handle Missing Values:** In this case,there were no missing values or nulls.
* **Data Standardization:** I normalized data formats (e.g., dates and time in a consistent format) to maintain consistency.

  ![image](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Power_Bi/assets/161952555/93b1248a-7048-492c-af69-8a876442e680)

  Snippet of data cleaning performed

  ## 3. Advanced Analytics and Insights
* **Key Metrics:** Calculated and analyzed key performance indicators (KPIs) such as total sales, total orders and total quantity by selected month by using the where function.
* **Segmentation Analysis:** Conducted segmentation analysis to understand sales patterns by store Location, store product category and store product type.


 ## 4. Data Import into Power BI
 * **Connection:** Established a direct connection between Power BI and the MySQL database to import cleaned and transformed data.
 * **Import Process:** Utilized Power BI Desktop to connect to MySQL, selecting relevant tables for analysis.

## 5. Data Modeling and Relationships (Power BI)
* **Data Modeling:** Created a new table called **Date Table** using the the calender function(CALENDAR(MIN(Transactions[transaction_date]), MAX(Transactions[transaction_date])) then created relationships between the transaction table and date table by dragging the date on the date table and joining it with the transaction_date on the transaction table.

![image](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Power_Bi/assets/161952555/997c646e-95ed-42b6-a4c5-dfc6edd2d3f5)

Snippet of New Table created

![image](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Power_Bi/assets/161952555/ac863c9e-d038-44d0-b2be-98a0207d61ae)

Snippet of Data Modelling


 * **Calculated Columns and Measures:** Defined calculated columns and measures (e.g. total sales,total orders total quantity, mom growth & diff sales etc ) using DAX (Data Analysis Expressions) in Power BI to facilitate analysis and i compared it to the the analysis i did using Mysql to check for accuracy. I uploaded a file where i displayed all calculation utilized using DAX.

## 6. Data Visualization and Analysis (Power BI)   
* **Dashboard Design:** Designed interactive dashboards in Power BI to visualize key metrics and insights.
* **Visualization Types:** Utilized various visualization types including bar charts, line charts, column charts and heat maps to represent sales performance across various category,products days and time.
* **Interactive Features:** Implemented slicers, filters, and drill-down capabilities in Power BI to allow stakeholders to explore data dynamically.

 ![image](https://github.com/Shevnon/Coffee_Shop_Sales_Mysql_and_Power_Bi/assets/161952555/a68f14d4-d0e1-4b6f-97d1-e5eeb6063446)

 Snippet of Final Dashboard
 

## 7. Advanced Analytics and Insights
* **Key Metrics:** Calculated and analyzed key performance indicators (KPIs) such as total sales, total orders and total quantity.
* **Segmentation Analysis:** Conducted segmentation analysis to understand sales patterns by store Location, store product category and store product type.

# KEY INSIGHTS
* The coffee shop had it's best sales during the month of June.
* There were more sales during the weekdays across all months.
* Hell's Kitchen recorded the most sales by location across all months.
* Coffee maintained the higest sales by store product category across all months while Barister Espresso is the best perfoming product type.

# CONCLUSION
It is important to monitor customer retention rates and make the necessary adjustment to enjoy continued patronage and the success of the business.

## RECOMMENDATIONS
1. Improve customer service.
2. Implement a loyalty program to reward repeat customers with discounts, freebies, or exclusive offers, incentivizing return visits.
3. Collaborate with local businesses, offices, or events to promote your coffee shop and reach new customers through partnerships or sponsorships.
4.  Host coffee tasting events, workshops, or themed promotions to attract customers and educate them about your coffee offerings.
5. Target persific demographic group.
6. Streamline operations to ensure quick service during peak hours. Consider mobile ordering options or drive-thru services for added convenience.
7. Collect feedback from customers regularly to understand their preferences and areas for improvement. Use this data to refine your offerings and services.

   
