# Sales Insight Data Analysis Dashboard

Welcome to the **Sales Insight Data Analysis Dashboard** repository! This Power BI dashboard provides a comprehensive analysis of sales data, offering valuable insights into sales performance, trends, and patterns to support strategic business decisions.

## Table of Contents
- [About the Dashboard](#about-the-dashboard)
- [Features](#features)
- [Data Model](#data-model)
- [Dashboard Overview](#dashboard-overview)
- [Setup and Installation](#setup-and-installation)
- [Data Cleaning and Transformation](#data-cleaning-and-transformation)
- [Usage](#usage)
- [License](#license)

---

### About the Dashboard

This Power BI dashboard was created to help visualize key sales metrics and understand the underlying trends within the data. It is suitable for teams looking to monitor and analyze their sales data for better decision-making, including performance tracking, sales growth analysis, and product category insights.

### Features

- **Sales Overview**: Provides a high-level view of total sales, revenue trends, and year-over-year (YoY) growth.
- **Product Category Insights**: Breaks down sales by product category, revealing top-performing categories and those with growth potential.
- **Geographic Analysis**: Visualizes sales distribution across regions or countries, identifying high-revenue areas.
- **Salesperson Performance**: Highlights performance metrics for each salesperson, including individual sales contributions and targets.
- **Time-based Trends**: Offers insights into seasonal or monthly sales trends to identify patterns and peak sales periods.
- **Interactive Filters**: Enables users to drill down into specific data points, view details by category, region, or time period, and uncover granular insights.

### Data Model

The dashboard is built on a well-structured data model that includes tables such as:
- **Sales Transactions**: Contains details of each sale, including date, amount, product, and region.
- **Product Details**: Includes product IDs, categories, and prices.
- **Salespersons**: Contains information on each salesperson, including their name, region, and ID.

Each table is connected based on relationships that ensure data accuracy and enable a seamless, integrated experience within the dashboard.

### Dashboard Overview

1. **Main Page**: An overview of the key performance indicators (KPIs) such as total sales, revenue growth, and YoY comparisons.
2. **Product Analysis**: Focuses on product-level insights, helping to identify high- and low-performing items.
3. **Salesperson Analysis**: Includes performance metrics and comparisons across the sales team.
4. **Time Analysis**: Showcases sales trends over time, highlighting seasonal variations and monthly performance.
5. **Geographic Analysis**: Maps sales by region to illustrate distribution patterns across locations.

### Setup and Installation

To use this dashboard, please ensure you have the following:

- **Power BI Desktop**: Download the latest version of Power BI Desktop from the [official Microsoft Power BI website](https://powerbi.microsoft.com/desktop/).
- **Sales Data File**: This dashboard is designed to work with the included dataset or with your own structured sales dataset. Ensure your data aligns with the model used in the dashboard.

**Steps:**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/sales-insight-data-analysis.git
2. **Open the Dashboard**:
Open the .pbix file in Power BI Desktop.
Connect Data Sources (if using a custom data source):
Go to Transform Data > Data Source Settings to update data connections.
Data Cleaning and Transformation
Before visualizing the data in Power BI, the following data cleaning and transformation steps were performed to ensure data quality and usability:

## Data Cleaning:

- **Handling Missing Values**: Missing or null values in key columns such as Product ID, Region, and Sales Amount were reviewed. Missing values were either imputed with appropriate means or medians or, where necessary, removed to maintain data integrity.
- **Removing Duplicates**: Duplicate records were identified and removed, particularly in tables like Sales Transactions to avoid over-representation in the data.
- **Standardizing Formats**: Ensured consistent date formats across all date columns, ensuring correct functionality in time-based visualizations. Text columns, such as product names and regions, were also standardized for consistent formatting.
## Data Transformation:

- **Data Type Conversion**: Correct data types were applied to each column:
Date columns were converted to Date data types.
Sales Amount and Revenue columns were converted to decimal or currency formats.
- **Creating Calculated Columns**: Calculated columns were added to support analysis:
- **Yearly and Monthly Breakdown**: Added columns for Year, Quarter, and Month to enable flexible time-based analysis.
- **Sales Margin Calculation**: Added a calculated column to measure sales margins based on sales and cost data (if available).
- **Creating Measures**:
Defined measures for key performance indicators, such as Total Sales, Average Sales Price, YoY Growth percentages, and Monthly Sales Change, using DAX formulas.
- **Creating Relationships**:
Set up relationships between tables, such as linking Sales Transactions to Product Details using Product ID, and to Salespersons using Salesperson ID. Relationships were defined as one-to-many to maintain data consistency and enable accurate filtering in visualizations.

## Data Aggregation:
Aggregated data where necessary, such as grouping sales by Product Category or Region for high-level insights.
Adding Hierarchies: Created hierarchies for time (Year > Quarter > Month) and for geographic drill-downs to allow users to explore data at different levels of detail.
Usage
Once opened in Power BI Desktop:
- **View and Interact**: You can explore each page of the dashboard, use filters, and drill down into specific insights.
---

## Technologies Used
- **Programming Languages**: Python, Dax
- **Software**: Mysql workbench, Power Bi

This `README.md` file is now ready for use in your GitHub repository. Let me know if you need any further customization!
