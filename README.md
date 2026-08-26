**Project Title**

**Sales Performance Analysis Dashboard using Microsoft Excel**

**Project Overview**
This project analyzes a sales dataset using Microsoft Excel to understand sales performance, product performance, salesperson performance, regional sales, and overall business trends.
The project covers the complete data-analysis workflow, starting from raw sales data and data cleaning and ending with an interactive sales dashboard using PivotTables, charts, KPI cards, and slicers.

**Project Objectives**
**The main objectives are to:**

1. Clean and prepare raw sales data.
2. Calculate total sales from quantity and unit price.
3. Analyze sales performance using Excel formulas.
4. Create sales KPIs.
5. Summarize data using PivotTables.
6. Compare salespeople, products, categories, and regions.
7. Visualize sales performance using charts.
8. Create an interactive dashboard.
9. Use slicers for filtering and analysis.
10. Present business insights in an easy-to-understand format.


**Dataset**

The dataset contains the following columns:

| Column        | Description                                 |
| ------------- | ------------------------------------------- |
| `Order_ID`    | Unique identification number for each order
|
| `Date`        | Date of the sale        
|
| `Salesperson` | Person responsible for the sale  
|
| `Product`     | Product sold 
|
| `Category`    | Product category 
|
| `Region`      | Sales region 
|
| `Quantity`    | Number of units sold 
|
| `Unit_Price`  | Price of one unit 
|
| `Total_Sales` | Total value of the sale   
|

**Total Sales Calculation**
The project calculates:
=Quantity*Unit_Price

**Data Cleaning**

The raw data was checked and cleaned before analysis.

Duplicate removal
Used:
Data → Remove Duplicates
This prevents the same order from being counted multiple times.

**Missing values**
Used:=COUNTBLANK(C2:C22)
to identify empty cells.

**Removing extra spaces**
Used:=TRIM(C2)
to remove unnecessary spaces from text.

**Standardizing text**

Used:=PROPER(C2)
to maintain consistent capitalization.

**Other functions practiced**:
=UPPER(C2)
=LOWER(C2)

**Number validation**
Used:
=ISNUMBER(H2)
to check whether values are stored as numbers.

Converting text to numbers
=VALUE(H2)

**Date Functions**
Date data was checked and analyzed
=YEAR(B2)
=MONTH(B2)
=DAY(B2)

**Number & Currency Formatting**
Unit_Price and Total_Sales were formatted as Indian currency.

Example custom format:
₹#,##0

**Excel Formulas Used
Basic functions:**
=SUM(I2:I22)
=AVERAGE(I2:I22)
=COUNT(I2:I22)
=COUNTA(A2:A22)
=MIN(I2:I22)
=MAX(I2:I22)
These were used to calculate important sales statistics.

**Logical Functions**

The project also practiced:

IF

=IF(I2>=50000,"High","Low")

IFS

=IFS(
I2>=75000,"Excellent",
I2>=50000,"Good",
I2>=25000,"Average",
I2<25000,"Low"
)

**AND**

Used to check whether multiple conditions are true.

**OR**

Used when any one of multiple conditions can be true.
These functions were used to create sales performance categories.

**Conditional Functions**

The project includes:
=COUNTIF()
=SUMIF()
=COUNTIFS()
=SUMIFS()

**Lookup Functions**

The project also covered:
XLOOKUP
VLOOKUP
INDEX-MATCH
These functions can be used to retrieve information from the sales dataset based on a matching value such as Order_ID or Product.**

**PivotTables**

Separate PivotTables were created to summarize the sales data.

**Sales by Salesperson**

Rows: Salesperson
Values: Sum of Total_Sales

Used to identify salesperson performance.

**Sales by Region**

Rows: Region
Values: Sum of Total_Sales

Used to compare regional performance.

**Sales by Product**

Rows: Product
Values: Sum of Total_Sales
SC Quality by produc .png
Used to identify products generating the highest sales.

**Quantity by Product**

Rows: Product
Values: Sum of Quantity
Used to understand product demand.

**Charts**

Charts were created from the PivotTables.

**Sales by Salesperson**

**Column Chart**

Used to compare salesperson performance.

**Sales by Region**

**Pie/Donut Chart**

Used to understand the contribution of each region.

**Sales by Product**

**Bar Chart**

Used to compare product sales.

**Sales Trend**

**Line Chart**

Used to visualize sales over time.

 **Sales KPIs**

The dashboard includes important sales KPIs.
QC Calculations.png

**Total Sales**
=SUM('Sales dataset'!I2:I22)

**Total Orders**
=COUNTA('Sales dataset'!A2:A22)

**Total Quantity**
=SUM('Sales dataset'!G2:G22)

**Average Sales**
=AVERAGE('Sales dataset'!I2:I22)

**Slicers**

Slicers were added to make the analysis interactive.

**The project uses slicers for:**

Salesperson
Region
Category
Product

Slicers allow the user to select a particular value and filter the PivotTable analysis.
QC Slicers.png

**Dashboard**

A separate Dashboard worksheet was created to present the main results visually.
QC Dashboard.png

**The dashboard contains:**

KPI Cards
otal Sales
Total Orders
Total Quantity
Average Sales
Charts
Sales by Salesperson
Sales by Region
Sales by Product
Sales Trend
Interactive Filters
Salesperson
Region
Category
Product

**Workbook Structure**

The Excel workbook is organized approximately as:
Sales Analysis Workbook

**Sales dataset**

**Pivot - Salesperson**

**Pivot - Region**

**Pivot - Product**

**Pivot - Quantity**

**Detail / Calculations**

**Dashboard**

**Tools & Skills Used**

**Tool:**

**Microsoft Excel**

**Data Analysis:**

Data Cleaning
Data Formatting
Sorting
Filtering
KPI Analysis
PivotTables

**Excel Functions:**

SUM
AVERAGE
COUNT
COUNTA
MIN
MAX
IF
IFS
AND
OR
COUNTIF
SUMIF
COUNTIFS
SUMIFS
XLOOKUP
VLOOKUP
INDEX-MATCH
TRIM
PROPER
UPPER
LOWER
VALUE
TEXT
YEAR
MONTH
DAY
DATE
TODAY
EOMONTH
DAYS


**Visualization:**

Column Charts
Bar Charts
Pie/Donut Charts
Line Charts
KPI Cards
Slicers
Interactive Dashboard


