**Sales Data Analysis Project Report**


**Objective**

The purpose of this project was to analyze sales performance using structured data stored in CSV files. The
analysis focused on product sales, regional performance, salesperson effectiveness, category breakdowns,
and temporal trends using SQL and Python in Google Colab.

**Datasets Used**

- Product.csv Product metadata (names, categories, costs)
- Region.csv Regional and territorial sales data
- Reseller.csv Reseller business details
- Targets.csv Monthly sales targets by employee
- Salesperson.csv Sales employee information
- SalespersonRegion.csv Employee-to-region mapping
- Sales.csv Transactional sales data
  
**Data Preparation**

All datasets were read using pandas with tab delimiters. Currency fields (Sales, Cost, Unit Price, etc.) were
cleaned using regex and converted to floats. OrderDate was converted to datetime format. Merges were
done using ProductKey, SalesTerritoryKey, and EmployeeKey to create a unified dataset.

**SQL Analysis**

An SQLite database was created in memory and populated with cleaned data. Key queries included:
- Sales Overview (total sales, cost, profit)
- Top-Selling Products
- Sales by Region
- Salesperson Performance
- Category-Level Insights
- Monthly Sales Trends

**Visualizations Created**

Charts were generated using Matplotlib and saved as PNGs in the charts/ directory. These include:
- Top-Selling Products
- Sales by Region
- Sales by Salesperson
- Category-Level Sales
- Monthly Sales Trends

**Key Insights**

- High-end products and accessories contributed significantly to revenue
- The Northwest and Central regions were top performers
- Some salespeople achieved significantly higher sales
- Monthly sales trends suggest seasonal patterns

**Conclusion**

This project demonstrates how to extract business insights from structured sales data using SQL, Python,
and visual reporting. The final PDF deliverable consolidates all analyses for presentation and review.
