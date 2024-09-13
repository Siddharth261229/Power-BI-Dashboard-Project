Maven Market Power BI Dashboard
Dashboard Link: Dashboard Link
Problem Statement
This dashboard provides valuable insights into Maven Market's business operations, helping the organization understand sales performance, customer demographics, product profitability, and store-level analysis. It allows the company to identify key areas of improvement, optimize product offerings, track revenue targets, and understand customer purchasing trends across various stores and regions.

By using this dashboard, Maven Market can also monitor their KPIs, track return rates, identify top-selling brands, and ultimately make data-driven decisions to enhance business growth and customer satisfaction.

Steps Followed
Step 1: Data Import

Imported datasets from multiple CSV files into Power BI Desktop, including:
MavenMarket_Customers
MavenMarket_Products
MavenMarket_Stores
MavenMarket_Regions
MavenMarket_Calendar
MavenMarket_Returns
MavenMarket_Transactions (1997 & 1998)
Step 2: Data Preparation

Cleaned and transformed data using Power Query Editor:
Promoted headers for each table.
Corrected data types (e.g., numerical fields for IDs, text for postal codes).
Extracted the birth year and merged customer names into a full name column.
Generated new calculated columns for key business attributes such as discount prices, years since store remodel, customer age, and other demographics.
Step 3: Data Profiling

Checked the data quality using the "Column Quality," "Column Distribution," and "Column Profile" options in the Power Query Editor.
Ensured data profiling was done on the entire dataset to ensure accurate analysis.
Step 4: Data Modeling

Created relationships between tables:
One-to-many relationships were established between Transaction_Data and the lookup tables (Customers, Products, Stores, Calendar).
Configured snowflake schema by connecting Stores and Regions.
Properly formatted the date and numeric fields and removed unnecessary columns to optimize the data model.
Step 5: DAX Calculations

Created several calculated columns and measures using DAX for business insights, including:
Quantity Sold, Quantity Returned, Total Transactions, and Total Revenue.
KPIs such as Return Rate (%), Profit Margin, and YTD Revenue.
DAX expressions for complex calculations such as revenue trends, sales by product, and region-wise performance.
Step 6: Dashboard Visualizations

Added multiple visuals to represent the data, including:
A matrix showing total transactions, profit margin, and return rate by product brand.
KPI cards displaying Total Transactions, Total Revenue, Total Profit, and Return Rate.
A map visual to show store-level performance across different regions.
Bar and column charts to display weekly revenue trends and a treemap for store locations.
Slicers for filtering the data by product category, store, region, and date.
Step 7: Filters and Slicers

Applied filters and slicers for enhanced user experience:
Slicers for product brands, store locations, customer demographics, and time periods.
Created interactive visuals where selections in one visual automatically filter others for in-depth data exploration.
Step 8: Advanced Formatting

Added conditional formatting to enhance the visibility of key metrics:
Data bars and color scales to represent profit and returns trends.
Highlighted high-performing products with green and underperforming ones with red.
Step 9: Additional Features

Bookmarks and notes were added to highlight key insights in the dashboard.
Text boxes and shapes were inserted for titles, company logo, and tagline for branding the dashboard.
Step 10: Calculated Columns and Measures

Created custom calculated columns:
Age group segmentation for customers.
Price tiers for products.
New measures to track total revenue, profit, and customer count using DAX expressions:
Customer Count: COUNT(MavenMarket_Customers[CustomerID])
Revenue Target Achievement: IF([Revenue] >= [Target], "Achieved", "Below Target")
Step 11: Publishing

After completing the design and testing, the dashboard was published to Power BI Service for business users to access and interact with the data in real-time.
Key Skills Demonstrated:
Data Transformation: Used Power Query to clean and transform raw data into usable formats for reporting.
Data Modeling: Created relationships between tables, ensuring efficient and logical data models.
DAX Calculations: Developed complex DAX measures for business insights, KPIs, and advanced filtering.
Interactive Dashboards: Built visually appealing and interactive dashboards with various visuals like cards, maps, and bar charts.
Power BI Service: Published reports to Power BI Service for easy access and real-time analysis.
Project Outcome:
The Maven Market dashboard helped the business identify key sales trends, understand customer demographics, and optimize product offerings. Through the use of various visualizations, the company can track performance metrics such as sales volume, return rates, and profitability at both the product and store level.

The dashboard provides a clear and concise view of Maven Market’s overall performance, assisting in decision-making for future growth strategies.

File Saved As:
MavenMarket_Report.pbix
