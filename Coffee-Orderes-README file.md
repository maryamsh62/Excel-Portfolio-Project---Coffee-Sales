# Coffee Sales Dashboard (Excel)

This project displays an interactive Excel dashboard for exploring coffee sales performance over time by country, product type, and customer segment. It walks through the complete workflow—from raw transactional data to a dynamic, user-friendly dashboard built with modern Excel features.


---

## Dashboard Preview

![Coffee Sales Dashboard](https://github.com/maryamsh62/Excel-Portfolio-Project---Coffee-Sales-Dashboard/blob/main/Coffee_Sales_Dashboard.png)

### Dataset
The project is based on a transactional dataset of coffee orders stored in the coffeeOrdersData.xlsx workbook.

### Tables
The workbook contains **three main tables**:

### 1. orders
1000 rows & 16 columns

**Key fields:**
- Order ID
- Order Date
- Customer ID
- Product ID
- Quantity
- Customer Name
- Email
- Country
- Coffee Type
- Roast Type
- Size
- Unit Price
- Loyalty Card

**Calculated columns**:
- Sales = Unit Price × Quantity
- Coffee Type Name / Roast Type Name – full descriptive names to make the dashboard slicers more readable.


### 2. customers
1000 rows & 9 columns

**Fields:**
- Customer ID
- Customer Name
- Email
- Phone Number
- Address Line 1
- City
- Country
- Postcode
- Loyalty Card 

### 3. products
48 rows & 7 columns

**Fields:**
- Product ID
- Coffee Type 
- Roast Type 
- Size 
- Unit Price
- Price per 100g
- Profit

### Time Period
Orders span from **January 2019 to August 2022**, allowing multi-year trend analysis.


### This project highlights several key Excel skills:

✅ Converting raw ranges to structured tables for easier formulas and automatic PivotTable updates

✅ Using XLOOKUP (and traditional INDEX/MATCH as a fallback) to bring customer and product information into the orders table

✅ Creating calculated columns for:
- Sales amount per line item
- Readable coffee and roast type names for visuals

✅ Building multiple PivotTables:
- Total sales over time
- Sales by country
- Top customers by total spend

✅ Designing an interactive dashboard sheet with:

Slicers for:
- Year / Month
- Roast Type
- Package size
- Loyalty card 

### Dashboard Layout & Functionality
The Dashboard sheet is the main interface for exploring the data. It contains:

**Time Slicer (Order Date)**
- Horizontal period selector for months and years (2019–2022). Allows the user to quickly filter the entire dashboard to a specific month, year, or custom range. 

**Filter Slicers:**
- Roast Type Name: Dark, Medium, Light
- Size: 0.2 kg, 0.5 kg, 1.0 kg, 2.5 kg
- Loyalty Card: Yes, No

**Total Sales Over Time**
- A line chart displays monthly total sales by coffee type (Arabica, Robusta, Excelsa, Liberica), aggregating total sales by date and coffee type and allowing you to visually compare how each coffee performs over time.

**Sales by Country**
- A horizontal bar chart summarizes total sales by country, highlighting the dataset’s main markets: the United States, Ireland, and the United Kingdom.

**Top 8 Customers**
- A bar chart displays the top-spending customers and their total sales, making it easy to quickly identify key customers for loyalty or marketing campaigns.

**All visuals are fully connected to the slicers, so any change to the filters instantly updates the entire dashboard.**

### Data Preparation
First, loaded raw data into separate sheets: orders, customers, products.

**Data Enrichment**
1. Used XLOOKUP to pull customer details (name, email, country, loyalty card) into the orders table using Customer ID.
2. Used INDEX-MATCH to bring product details (coffee type, roast type, size, unit price) using Product ID.

**Created calculated columns:**
- Sales = Unit Price × Quantity
- Full descriptive labels for coffee and roast types to improve chart and slicer readability.

**Formatting Data**

Regarding data formatting, I applied a custom date format to the Order Date column so that days are shown with an abbreviated month name (dd-mmm-yyyy). Next, formatted the Size column to include the metric unit (kg), and set the Unit Price and Sales columns to display values in US dollars. At the end, I checked the dataset for duplicate values.


Then, converted ranges to Excel Tables to enable structured references and dynamic PivotTables.

## Result
The Coffee Sales Dashboard shows that the United States is by far the strongest market, generating roughly 35,600 dollars in sales, compared with about 6,700 dollars from Ireland and 2,800 dollars from the United Kingdom. Monthly sales fluctuate across the period, with noticeable spikes for different coffee types at various times, but all four types (Arabica, Robusta, Excelsa, Liberica) contribute meaningfully to revenue. The Top 8 Customers chart reveals a broad customer base: even the highest-spending customer contributes only a few hundred dollars in total sales, indicating that performance depends on many small to mid-size customers rather than a few large accounts. Using the slicers (roast type, size, loyalty card, and date), users can quickly drill into these patterns to see which product formats, markets, and customer segments drive sales over time.

### Purpose of the Project
This project is ideal for:
- Demonstrating Excel dashboard and data modeling skills in a portfolio
- Practicing data cleaning, lookup formulas, PivotTables, and dashboard design
- Providing a simple, realistic example of sales reporting for a small business
- Feel free to fork this project, adapt the dataset, or redesign the visuals to match your own style and learning goals.


### How to Use This Project
- Download the Workbook
- Clone the repository or download coffeeOrdersData.xlsx.
- Open in Excel
- Use Excel 365 or Excel 2019+ for full compatibility with XLOOKUP and modern charts.
- Older versions of Excel may require using the INDEX/MATCH version of formulas.








```python

```
