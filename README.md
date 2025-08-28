# Sales Analytics Report

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Process](#process)
- [Features](#features)
- [Insights](#insights)
- [Learning](#learning)

## Overview


Analyze 2014–2018 sales data to identify key revenue and profit drivers across products, channels, and regions; uncover seasonal trends and outliers; and align performance against budgets. Use these insights to optimize pricing, promotions, and market expansion for sustainable growth and reduced concentration risk.  

<img width="1479" height="804" alt="O2" src="https://github.com/user-attachments/assets/6b5d3513-dea3-4dc2-9517-63aed4e9b036" />

<img width="1474" height="809" alt="O3" src="https://github.com/user-attachments/assets/6ecf7c17-8335-4af2-992c-7edb046d3870" />

<img width="1473" height="810" alt="O4" src="https://github.com/user-attachments/assets/68ee4b15-cc95-498a-bf71-0aa644493dd9" />


## Dataset

Here are the descriptions for the given table headers shown in your images:

### 1.Sales Order Table

| Column Name                | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| OrderNumber                | Unique identifier for each sales order.                                     |
| OrderDate                  | Date when the order was placed.                                             |
| Customer Name Index        | Numeric index referencing the customer who placed the order.                |
| Channel                    | Sales channel type (e.g., Wholesale, Distributor, Export)                   |
| Currency Code              | Currency used for the transaction (e.g., USD).                              |
| Warehouse Code             | Identifier for the warehouse fulfilling the order.                          |
| Delivery Region Index      | Numeric index referencing the delivery region.                              |
| Product Description Index  | Numeric index referencing the product being ordered.                        |
| Order Quantity             | Number of units ordered.                                                    |
| Unit Price                 | Price per unit of the product.                                              |
| Line Total                 | Total value of the line (Order Quantity x Unit Price).                      |
| Total Unit Cost            | Total cost associated with the units in the order.                          |

### 2. Customer Table

| Column Name       | Description                                                              |
|-------------------|--------------------------------------------------------------------------|
| Customer Index    | Numeric reference for each customer, used to link with orders.           |
| Customer Names    | Name of the customer or business entity.                                 |

### 3. Region Table

| Column Name         | Description                                                         |
|---------------------|---------------------------------------------------------------------|
| id                  | Unique identifier for each city/location.                           |
| Name                | Name of the city/location.                                          |
| county              | Name(s) of the county or counties where the city is located.        |
| state_code          | Abbreviation for the state.                                         |
| state               | Full name of the state.                                             |
| type                | Type of locality (e.g., City).                                      |
| latitude            | Latitude coordinate of the location.                                |
| longitude           | Longitude coordinate of the location.                               |
| area_code           | Telephone area code(s) for the locality.                            |
| population          | Population count.                                                   |
| households          | Number of households in the locality.                               |
| median_income       | Median household income.                                            |
| land_area           | Land area .                                                         |
| water_area          | Water area .                                                        |
| timezone            | Time zone of the locality.                                          |

### 4. State Region Table

| Column Name     | Description                                                     |
|-----------------|-----------------------------------------------------------------|
| State Code      | Abbreviation for the state.                                     |
| State           | Full name of the state.                                         |
| Region          | The designated region for the state (e.g.,North, South etc.).   |

Here are the descriptions for the table headers shown in your provided images:

### 5. Product Table

| Column Name  | Description                                         |
|--------------|-----------------------------------------------------|
| Index        | Numeric identifier for each product.                |
| Product Name | Name of the product.                                |

### 6. Budget Table

| Column Name     | Description                                                                   |
|-----------------|-------------------------------------------------------------------------------|
| Product Name    | Name of the product (matches with Product Name in the index table).           |
| 2017 Budgets    | The allocated budget for the product for the year 2017 (numeric/currency).    |


## Process

Tools Used :- Microsoft Excel, Python, Jupyter Notebook, Microsoft Power BI.  

Process:-   
-Familiarizing with the dataset.  
-Uploading the dataset from CSV file to Python using Jupyter Notebook.    
-Performing Data Cleaning Operations.  
-Ensuring the correct data types for each field.  
-Performing EDA using Python.  
-Exporting the data-frame to an Excel file for further Analysis in Power BI.  
-Connecting the data to a Power BI file.    
-Generating required Column for analysis.  
-Checking Data Module.     
-Generating Calculations where required.  
-Designing a UI for Power BI dashboard.  
-Creating data visuals for the Power BI dashboard as per the design.  
-Formatting the Visuals.  
-Adding Slicers and other visuals as per the UI design.  

## Features

-UI designed Dashboard with Homepage and Button Navigation.  
-Bookmarks are used to hide the Filters/Slicers giving a clean look to the dashboard.   
-Consistent theme is followed throughout the report.  
-EDA using Python.  

## Insights

### **Executive Overview & Trends**
1. **Strong Financial Performance:**  
   - **Total Revenue:** $1.2 billion;  
   - **Total Profit:** $461.8 million (Profit Margin: 37.36%).
   - **Total Orders:** 64K, with an **average revenue per order** of about $19.3K.

2. **Seasonal Trends:**  
   - Both revenue and profit display seasonality, peaking in April, May, and September, with dips in February and July.

3. **Customer Spending:**  
   - Most orders are below $100K. There are few, but significant, high-value orders.

4. **Product Margins:**  
   - Profit margins remain largely above 30%, with some products achieving over 40% margin.

### **Product & Channel Performance**
5. **Top Products Drive Growth:**  
   - **Product 26** is the top seller ($117M), followed closely by Product 25 ($109M).  
   - However, the **highest margin product**, Product 9, earns a 40% profit margin.

6. **Revenue vs. Profitability:**  
   - High-revenue products do not always yield the highest margins, suggesting room for pricing or cost optimization.

7. **Sales Channels:**  
   - **Export channel** delivers the largest share of both revenue (54%) and profit (54%), outpacing Wholesale and Distributor.
   - Margins are comparable across channels, but Export leads slightly in efficiency.

### **Geographic & Customer Insights**
8. **Regional Revenue Leadership:**  
   - The **Midwest** is the largest region by revenue ($372.1M, 30.1% of total), while the **West** posts the strongest profit margin (37.5%).

9. **State Performance:**  
   - **California** generates the most revenue ($228.8M, 19.5% of total), while **Wyoming** has the lowest ($1.8M).
   - Illinois, Florida, Texas, and New York round out the top five revenue states.

10. **Key Customers:**  
    - **Aibox Company** is the top customer by revenue ($13M), but **Neutrogena Ltd** delivers the top margin (44.8%).

### **Additional Notable Points**
11. **Bottom Performers:**  
    - Wyoming, South Dakota, and DC are among the least contributing states by revenue.
    - The lowest-performing customers by profit margin still deliver margins over 30%, indicating an overall healthy margin profile.

12. **Consistency Across Regions:**  
    - Profit margins by region are relatively similar, ranging from 37.3% to 37.5%.

### **Summary**
- The business is profitable with strong margins.
- Power is concentrated among top products, top customers, and certain regions (especially Midwest and California).
- Export channels are the most efficient.
- Some revenue-heavy products may benefit from a focus on margin improvement.
- There are opportunities to improve under-performing regions and customer segments.


