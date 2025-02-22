# Advanced-Data-Analytics-for-Global-Electronics-Retailer-in-Excel
 sales analysis in Excel for a global electronics retailer, cleaning data, creating relationships, and designing an interactive dashboard to track revenue, orders, and trends for better decision-making.
GLOBAL ELECTRONICS RETAILER

# Advanced-Data-Analytics-for-Global-Electronics-Retailer-in-Excel

Sales analysis in Excel for a global electronics retailer, cleaning data, creating relationships, and designing an interactive dashboard to track revenue, orders, and trends for better decision-making.

## GLOBAL ELECTRONICS RETAILER

### 🔍 THE SITUATION
Data Analysis for Maven Electronics, a global retailer that sells computers, cell phones, TVs, cameras, appliances, and more, both online and in-store.

### ✏️ THE ASSIGNMENT
Revenue has been on a downward trend since 2020, and management needs help consolidating the data to conduct an exploratory analysis.  
The goal is to use the CSV files provided to build a data model and interactive report that the management team can use to explore performance.

### ✅ THE OBJECTIVES
- Profile and prepare the data  
- Build a relational data model  
- Enrich and explore the data  
- Build an interactive report  

## OBJECTIVE 1: PROFILE & PREPARE THE DATA
✔️ Connect to the Sales CSV file and profile the data. How many orders were recorded? Over what time period? Are there any interesting observations about delivery dates?  
• Add a TransactionKey field to uniquely identify each row  

✔️ Connect to the Products CSV file and profile the data. What does the company sell? How many distinct categories and subcategories are there?  

✔️ Connect to the Stores CSV file and profile the data. How many stores does Maven Electronics operate? Are there any that aren’t like the others?  

✔️ Connect to the Exchange_Rates CSV file and profile the data. What information does this table contain, and how could it be used?  

✅ Connect to the Customers CSV file and profile the data. How many customers has the company served? Where are customers primarily located?  
- Remove the Zip Code column  
- Transform the City field to capitalize the first letter of each word  
- Add a new column to calculate Customer Age in years, as a rounded whole number  
- Add a conditional column to calculate Age Range, based on the following logic:  
  - If Customer Age > 60, Age Range = Senior  
  - If Customer Age > 30, Age Range = Adult  
  - If Customer Age > 18, Age Range = Young Adult  

✅ Create a Calendar table that contains a list of contiguous dates (no gaps) and reflects the same date range as the Sales table  
- Add new columns for Day Name, Start of Week, Start of Month, Start of Quarter, and Year  

## OBJECTIVE 2: BUILD A RELATIONAL MODEL
✅ Create relationships from the Sales table to Customers, Stores, Products, and Calendar  

✅ What happens when connecting the Sales table to Exchange Rates? Add a new column to Sales and Exchange Rates tables named ExchangeKey and use that field to relate them via a 1:many relationship  

✅ Hide all foreign keys from the Sales table  

✅ Split the Products table into category and subcategory-level dimension tables, and update the data model to relate these new tables  

![Data Model](https://github.com/DE-romane/Advanced-Data-Analytics-for-Global-Electronics-Retailer-in-Excel/blob/main/Data%20%2B%20Project/Data%20Model.png)



## OBJECTIVE 3: ENRICH & EXPLORE THE DATA
✅ Add a blank, dedicated measures table  

✅ Create a new measure to calculate Total Orders, based on Order Number  
- How has order volume trended over time? Do all product categories show a similar trend?  

✅ Calculate Total Revenue (USD), based on Quantity and Unit Price (USD)  
- Which stores generate the most revenue? Which individual products?  
- BONUS: Create another version of Total Revenue to calculate revenue in local currency  

✅ Calculate Average Order Value (AOV), based on Total Revenue (USD) and Total Orders  
- How does AOV compare across product categories? Are there differences based on customer age?  

✅ Calculate Average Delivery Time, in days  
- Which types of products tend to be delivered fastest or slowest?

![Measures Table](https://github.com/DE-romane/Advanced-Data-Analytics-for-Global-Electronics-Retailer-in-Excel/blob/main/Data%20%2B%20Project/Measures%20Table.png)

## OBJECTIVE 4: BUILD AN INTERACTIVE REPORT
✅ Show orders, revenue, AOV, and average delivery time as KPI cards (or similar)  

✅ Show revenue by month as a line chart, and by Product Category as a bar chart  

✅ Add slicers for StoreKey and Year, connected to all cards and visuals  

✅ Adjust formatting and polish for clarity and readability  
- Use consistent colors and themes  
- Eliminate unnecessary details or chart elements  
- Update number formats for readability  

✅ What trends and patterns are visible? Where would deeper analysis be beneficial?

![Dashboard](https://github.com/DE-romane/Advanced-Data-Analytics-for-Global-Electronics-Retailer-in-Excel/blob/main/Data%20%2B%20Project/dashboard.png)

## 🚀 OUTCOME & IMPACT
The final report enabled management to identify revenue trends, explore customer behaviors, and optimize business decisions with an intuitive, data-driven approach.
