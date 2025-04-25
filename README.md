# Product-Sales-Dashboard

### Power BI Dashboard
![Product Sales Dashboard](https://github.com/Devanshi1206/Product-Sales-Dashboard/blob/main/Dashboard.png)
Here, SKU (Stock Keeping Unit) are the unique identity code of any product.

## Data Used

    Data - Product Sales Data with 400 rows

    Data Cleaning & Analysis - Power Query

    Data Visualization - Power BI

## Questions

1. What are the different KPI (Total Revenue, Total Profit, Number of Products Available)
2. What could be the possible slicers?
3. What are the top 10 products by Revenue?
4. Revenue Share by different Category (e.g., Electronics, Clothing)
5. Total Sales and Profit grouped by Colour
6. Average List Price & Cost per Model

## Summary of Findings
- The category with the highest sales is bicycles and their components.  
- Accessories yield the greatest profit margins, followed by clothing and components.  
- Items in black are the most frequently sold.  

## DAX queries used:

Total Revenue = sum(Product_data[List Price])

Total Cost = SUM(Product_data[Standard Cost])

Margins = Product_data[List Price] - Product_data[Standard Cost]

Profit_Margin = DIVIDE(SUM(Product_data[Margins]),SUM(Product_data[List Price]))*100

Number of Products = DISTINCTCOUNT(Product_data[ProductKey])

## Limitations

- Some data had black values, so they were removed from the visualisations since the data is relatively small.
