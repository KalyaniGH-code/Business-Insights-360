# Business-Insights-360

#PROJECT OVERVIEW

AtliQ Hardware has experienced significant growth in recent years and is now taking a strategic step toward implementing data analytics using Power BI for the first time. 
This initiative aims to provide stakeholders with valuable insights across key business functions such as finance, sales, marketing, and supply chain. 
By leveraging data-driven decision-making, the company seeks to gain a competitive edge in the market and drive continued success.

##Tech Stack
1. SQL – For querying and managing data

2. Power BI Desktop – Core tool for data visualization and report development

3. Excel – For preliminary data handling and validation

4. DAX (Data Analysis Expressions) – Used for creating measures and calculated columns

5. DAX Studio – For optimizing DAX queries and improving report performance

6. Project Charter Document – Guiding the project scope and objectives.

##Power BI Techniques Learned
1. Framing the right questions before initiating a project

2. Creating calculated columns to enrich datasets

3. Building dynamic measures using DAX

4. Designing efficient data models

5. Implementing bookmarks to toggle between visuals

6. Navigating between report pages using buttons

7. Utilizing the DIVIDE() function to handle division by zero scenarios

8. Generating date tables using M language

9. Creating dynamic titles based on user-applied filters

10. Using KPI indicators for performance tracking

11. Applying conditional formatting with icons and background colors

12. Validating data accuracy and integrity

13. Understanding and using Power BI Service

14. Publishing reports to the Power BI Service platform

15. Configuring personal gateways for scheduled data refreshes

16. Developing and publishing apps in Power BI

17. Managing collaboration, workspace organization, and user access in Power BI Service.

##Key Business Terms
1. Gross Price

2. Pre-Invoice Deductions

3.Post-Invoice Deductions

4. Net Invoice Sale

5. Gross Margin

6. Net Sales

7. Net Profit

8. COGS (Cost of Goods Sold)

9. YTD (Year to Date)

10. YTG (Year to Go)

11. Direct Sales

12. Retailers

13. Distributors

14. Consumers

##Company Background
AtliQ Hardware is a rapidly expanding global company that specializes in selling computers and computer accessories. It operates through three main channels: retailers, direct sales, and distributors.

Despite its growth, the company recently experienced unexpected losses after launching a store in America based solely on surveys, intuition, and basic Excel analysis. Meanwhile, competitors with well-established analytics teams have been leveraging data to make informed strategic decisions.

To stay competitive and avoid similar missteps in the future, AtliQ Hardware has recognized the urgent need to build a robust data analytics capability. By adopting tools like Power BI and focusing on data-driven decision-making, the company aims to gain deeper insights into its operations and improve business outcomes.

#Dataset Understanding
Before diving into analysis, it's crucial to first understand the structure and content of the data. A clear grasp of the available datasets will help guide meaningful insights and improve the overall quality of analysis.

##Types of Tables
Dimension Tables: Contain static, descriptive information such as customer details, market regions, and product specifications.

Fact Tables: Store transactional data, such as sales and forecasts, which are used for quantitative analysis.

##Database: gdb041
###dim_customer

- Covers 27 distinct markets (e.g., India, USA, Spain)

- Includes 75 unique customers across these markets

- Two platform types:

     1. Brick & Mortar – Physical/offline stores

     2. E-commerce – Online platforms (e.g., Amazon, Flipkart)

- Three sales channels:

     1. Retailer

     2. Direct

     3. Distributor

###dim_market

- Represents 27 distinct markets

- Divided into 7 sub-zones

- Spans across 4 regions:

   1. APAC

   2. EU

   3. LATAM

- Unassigned/Unknown (nan)

###dim_product

- Organized by divisions:

   1. P & A: Peripherals, Accessories

   2. PC: Notebooks, Desktops

   3. N & S: Networking, Storage

- Contains 14 product categories (e.g., internal HDD, keyboard)

- Includes multiple product variants for each category

###fact_forecast_monthly

- Provides monthly customer demand forecasts

Benefits:

Improves customer satisfaction

Reduces warehousing costs

This table is denormalized to optimize analytical performance

All dates are standardized to the first day of the month

The final column contains forecasted quantities

fact_sales_monthly

Similar structure to fact_forecast_monthly

The final column shows actual sold quantities

##Database: gdb056
###freight_cost

- Contains logistics costs for each market by fiscal year

###gross_price

- Lists gross product prices, identified by product code

###manufacturing_cost

- Records product manufacturing costs by year and product code

###pre_invoice_deductions

- Details pre-invoice deduction percentages per customer and year

###post_invoice_deductions

- Includes information about post-invoice and additional deductions

## Importing Data into Power BI
- Since the project utilizes a MySQL database, data is imported into Power BI by connecting directly to the MySQL server using valid database credentials.

###Data Modeling
1. Data modeling is a foundational step in Power BI development. A well-designed model ensures optimal performance and meaningful visualizations.

2. All report visuals are built on top of this model.

3. Poor data modeling can lead to:

4. Slow report performance

5. Inaccurate insights

6. Difficulty in maintaining the dashboard

