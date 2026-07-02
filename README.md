# E-Commerce-Sales-Analysis-Using-python
The primary objective of this project is to evaluate product and category performance to optimize inventory and sales strategies.

An analytical data project focused on cleaning, reconstructing, and analyzing e-commerce sales transactions from the GCC region. This project processes raw transactional data to fix data quality issues, extract key performance indicators (KPIs), and deliver actionable business intelligence

The analysis handles a dataset of 100 transaction records with 7 key attributes:
* `Order_ID`
* `Product`
* `Category`
* `Quantity`
* `Price`
* `Revenue`
* `Order_Date`

## Data Cleaning & Transformation
Before conducting the analysis, the following data preprocessing steps were executed:
1. **Handling Missing Values:** Identified 34 missing entries within the `Revenue` column. These gaps were programmatically resolved by calculating:
   $$\text{Revenue} = \text{Quantity} \times \text{Price}$$
2. **Date Standardization:** Converted the `Order_Date` text column into a standardized datetime format for consistent time-series tracking.
3. **Feature Engineering:** Extracted a dedicated `Month` column from the standardized dates to enable monthly sales aggregations.

## Key Insights
* **Data Completeness:** Missing revenue values were successfully calculated using Quantity × Price, ensuring a complete and accurate baseline for analysis.
* **Category Performance:** Food products contributed significantly more revenue than Dairy products, establishing Food as the primary driver of total sales.
* **Revenue Concentration:** Revenue distribution shows that a few products account for a large portion of total sales, indicating high reliance on specific items.
* **Top Product:** Rice generated the highest revenue among all products, making it the top-performing product in the dataset.

## Business Recommendations
* **Inventory Management:** Increase inventory levels for Rice and other top-performing products to avoid stock shortages and capture all market demand.
* **Targeted Marketing:** Introduce promotional campaigns for lower-performing products to improve sales momentum and balance stock turnover.
* **Demand Forecasting:** Monitor sales trends regularly to identify peak demand periods and optimize proactive stock planning.
* **Strategic Pricing:** Create product bundles and targeted discounts to increase average order value (AOV) across the platform.

## Technologies Used
* **Python** 
* **Pandas** (Data cleaning and aggregation)
* **Matplotlib** (Data visualization)
* **Jupyter Notebook** (Development environment)

```
