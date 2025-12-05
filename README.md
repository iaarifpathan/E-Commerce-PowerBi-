# E-Commerce Sales & Order Performance Dashboard
#### A complete analytical dashboard providing deep insights into sales performance, order behavior, customer distribution, and sales target tracking across countries, teams, and managers.
### 1. Business Problem
#### A global e-commerce company wants to analyze:
* Sales performance across teams and managers
* Order patterns & customer demographics
* Target achievement vs actual revenue
* Country-wise growth opportunities
* Sales channel efficiency
### 2. Project Overview
#### This Power BI project analyzes global e-commerce performance using 5 interactive dashboard pages:
#### 1. Sales Team Performance
#### 2. Orders Dashboard
#### 3. Sales Targets & Goal Tracking
#### 4. Sales Distribution Across Countries
#### 5. Sales Manager Performance by Country
#### The dashboard helps stakeholders understand sales efficiency, customer behavior, order trends, and regional growth opportunities.
### 3. Tools & Technologies
* Power BI Desktop
* Power Query (Data Cleaning & Shaping)
* DAX (Measures & KPIs)
* Data Modelling
* Maps Visualization (Azure Maps / Bing Maps)
* CSV Data

<mark>Sales Team</mark>
<img width="990" height="557" alt="Sales_Team" src="https://github.com/user-attachments/assets/025347bd-1388-4936-a64b-dc0913d978a0" />

### Page 1 — Sales Team Dashboard
#### KPIs:
* Total Sales
* Total Orders
* Average Sales Difference
Visuals:
* Sales by POC (Target Performance)
* 2023 Sales Target by Team
* Country-wise Top Sales Managers
* Top-10 Sales Managers (Sales Value)
* Top-10 POCs (Sales Value)
* Sales Manager Ranking by Orders & Customers
#### Insights:
* Identified best-performing managers and POCs
* Team Alpha shows the highest target achievements
* USA contributes the largest share in order revenue

<mark>Orders</mark>
<img width="995" height="561" alt="orders" src="https://github.com/user-attachments/assets/a9d28986-c13a-478e-ba68-97a127390586" />

### Page 2 — Orders Dashboard
#### KPIs:
* Total Orders
* Average Order Value
* Top Country by Orders
* Top Order Source
#### Visuals:
* Customer Count by Gender
* Orders by Category
* Monthly Order & Revenue Trend
* Top 10 Customers by Order Value
* Orders by Country & Order Source
* Customer Count by Top Countries
* Average Order Value by Top Countries
#### Insights:
* Website generates the highest number of orders
* USA ranks #1 in order volume
* October & November show peak order activity

<mark>Sales Target</mark>
<img width="990" height="558" alt="Sales_Target" src="https://github.com/user-attachments/assets/d6f62309-c1b0-41a0-b5fd-558f13a74cc2" />

### Page 3 — Sales Target Dashboard
#### Visuals:
* Sales Manager, POC, Team slicers
* Date Slicer
* Average Sales vs. Target Trend (KPI + Line background)
#### Insights:
* Sales remained below target by approx 21.7%
* Consistent underperformance across several teams
* Clear visual to track daily target gaps

<mark>Sales in each country</mark>
<img width="991" height="555" alt="Sales_in_each_country" src="https://github.com/user-attachments/assets/ccb96999-6e9c-4299-ac76-edf223a3d073" />

### Page 4 — Sales in Each Country
#### Visuals:
* Global map showing sales value by country
#### Insights:
* USA, Germany, France, India, and Singapore are top-performing regions
* Regional managers show strong contribution to revenue
* Geographic insights highlight expansion opportunities

<mark>SM Sales by Country</mark>
<img width="988" height="553" alt="SM_Sales_by_country" src="https://github.com/user-attachments/assets/53491593-4823-44d1-9216-b2ec295140fe" />

### Page 5 — Sales Manager Sales by Country
#### Visuals:
* Detailed matrix of Sales Manager × Country × Order Value
#### Insights:
* Provides complete view of each manager’s international performance
* Benjamin Chen and Noah Meier lead in multiple countries
* Useful for manager evaluation & incentive planning

### DAX Measures Used
#### (Some examples from your project)
* Total Sales = SUM(Sales[SalesValue])
* Total Orders = DISTINCTCOUNT(Orders[OrderID])
* Average Sales Difference = AVERAGE(Sales[SalesValue] - Sales[Target])
* Target Bucket = SWITCH(TRUE(), ...)
* Sales Manager = RELATED('Sales Targets'[Sales Manager])

### Data Cleaning (Power Query)
* Removed duplicates
* Corrected data types
* Extracted date, month, year
* Handled null and inconsistent values
* Standardized category & country names
* Merged tables using keys (POC, Manager, Country)

### Key Insights Summary
* USA is the strongest market across both sales and orders
* Website is the top-performing sales channel
* Top-performing managers: Benjamin Chen, Noah Meier, Alexander Müller
* Sales underperformed target by 21%
* Strong customer base evenly split across genders
* Seasonal order peaks in October–November

### Conclusion
#### This dashboard provides a complete 360° performance view for business decision-makers, helping them monitor:
* Sales health
* Order patterns
* Customer demographics
* Geographic performance
* Manager efficiency
* Target achievement
