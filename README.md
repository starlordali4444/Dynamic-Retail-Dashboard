# Dynamic Retail Dashboard

## Objective
The primary goal of this project is to develop a comprehensive and dynamic dashboard for analyzing retail data. By leveraging various KPIs and visualizations, the dashboard aims to provide insights into sales performance, profitability, product trends, and return analysis. This project is designed to facilitate better decision-making for retail managers and stakeholders by presenting key metrics in an intuitive and interactive way.

## Significance
Retail businesses thrive on accurate data analysis and insights. The dynamic retail dashboard serves as a powerful tool for:

- **Tracking KPIs**: Monitor crucial metrics like total sales, total profit, order count, and profit margin.
- **Understanding Sales Trends**: Analyze sales trends over time, identify top-performing regions, and assess the effectiveness of different segments.
- **Product Analysis**: Evaluate which product categories and subcategories drive the most sales and profit.
- **Customer Analysis**: Identify top and bottom customers to tailor strategies and optimize engagement.
- **Return Analysis**: Understand return patterns across different markets and segments.

## Data Sources
The dashboard integrates data from three tables:

1. **Orders**: Contains detailed order information, including sales, profit, quantity, category, and market data.
2. **People**: Contains information about individuals and their assigned regions.
3. **Return**: Tracks returned orders along with the corresponding markets.

### Sample Data
**Orders Table:**
| Order ID | Order Date | Ship Date | Ship Mode | Customer ID | Customer Name | Segment | Country | Market | Sales | Quantity | Discount | Profit | Order Priority |
|----------|------------|-----------|-----------|-------------|---------------|---------|---------|--------|-------|----------|----------|--------|----------------|
| CA-2012-124891 | 31-07-2020 | 31-07-2020 | Same Day | RH-19495 | Rick Hansen | Consumer | United States | US | 2309.65 | 7 | 0 | 762.18 | Critical |

**People Table:**
| Person         | Region   |
|----------------|----------|
| Anna Andreadi  | Central  |
| Chuck Magee    | South    |

**Return Table:**
| Returned | Order ID | Market        |
|----------|----------|---------------|
| Yes      | MX-2013-168137 | LATAM |

## Problem Statements Addressed
The dashboard solves the following problem statements:

1. **KPI Calculation**: Calculates total sales, total profit, total quantity, number of orders, and profit margin.
2. **Sales and Profit Analysis**: Provides a detailed analysis of sales and profit across different regions, markets, and segments.
3. **Category-wise Profit**: Displays profit contribution by different product categories.
4. **Segment-wise Sales Share**: Shows the share of sales across different customer segments.
5. **Sales by Country**: Highlights sales distribution by country.
6. **Top 5 Subcategories**: Identifies subcategories with the highest sales.
7. **Bottom 5 Subcategories**: Highlights subcategories with lower sales.
8. **Yearly Sales Trend**: Visualizes sales trends over time to identify seasonal patterns.

### Next Steps
The future enhancements for this project include:

- **Return Analysis**: Explore the reasons behind returns and analyze trends across markets.
- **Top and Bottom Customer Analysis**: Identify key customers and those requiring engagement strategies.
- **Segment Analysis**: Deep dive into customer segments to tailor marketing and sales strategies.
- **Market Analysis**: Compare sales and returns across different markets to optimize regional performance.
- **Product Analysis**: Examine product-level performance to optimize inventory and pricing strategies.

## KPI Metrics
A dynamic KPI table was created to streamline the dashboard’s metrics:

| Name               | Metric                 | Symbol |
|--------------------|------------------------|--------|
| Total Sales        | Sum of Sales           | 💰     |
| Total Profit       | Sum of Profit          | 📈     |
| Total Quantity     | Sum of Quantity        | 📦     |
| No of Orders       | Count of Order ID      | 🛒     |
| Profitability      | Sum of Profitability   | 💹     |
| Average Discount   | Average of Discount    | 🔍     |

## Steps to Create the Dashboard

1. **Set Up Your Environment**:
   - Choose a data analysis and visualization tool such as **Tableau**, **Power BI**, or **Python** with **Plotly/Dash**.
   - Prepare your **development environment** by installing necessary libraries or software.
   - Load the **Orders**, **People**, and **Return** datasets into your environment.

2. **Data Cleaning and Preparation**:
   - Ensure that each dataset is **cleaned** for null values, duplicates, and formatting inconsistencies.
   - **Join** the three tables as needed, such as using `Order ID` to match returns data with orders.
   - Create derived fields like **Total Profit**, **Profit Margin**, and **Sales Contribution**.

3. **KPI Calculation**:
   - Calculate **Total Sales**, **Total Profit**, **Total Quantity**, **Number of Orders**, and **Average Discount**.
   - Summarize these metrics in a **KPI table** to be used in the dashboard.

4. **Data Visualization**:
   - Create various **charts and graphs**:
     - **Bar Charts** for top and bottom subcategories.
     - **Line Charts** for visualizing the **Yearly Sales Trend**.
     - **Pie Charts** for **Segment-wise Sales Share**.
     - **Geo Maps** for **Sales by Country**.
   - Use **filtering options** to allow users to filter data by **region, market, and customer segment**.

5. **Return Analysis**:
   - Visualize the number of returns across different **markets** and **product categories**.
   - Provide insights into patterns and potential issues causing returns.

6. **Deploy the Dashboard**:
   - Publish the dashboard to a web server (if using a tool like Tableau or Power BI) or **deploy it using Python** (e.g., Dash app on a cloud service).
   - **Share access** with stakeholders by providing a link or embedding the dashboard on a web page.

7. **Test and Iterate**:
   - **Test** the dashboard for functionality and usability.
   - Gather **feedback** from users and **iterate** to improve user experience and insights.

## Conclusion
This dynamic retail dashboard offers a comprehensive solution for analyzing retail data, providing valuable insights into sales, profitability, and customer behavior. By focusing on the key metrics and offering a user-friendly interface, the dashboard is an effective tool for retail managers to make data-driven decisions. Future enhancements like return analysis and market analysis will further strengthen its capabilities, making it an indispensable asset for retail businesses.
