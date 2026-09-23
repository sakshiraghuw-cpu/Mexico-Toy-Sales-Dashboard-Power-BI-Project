# Mexico Toy Sales Dashboard | Power BI Project

## Project Overview

The Mexico Toy Sales Dashboard is an end-to-end Business Intelligence solution developed in Power BI to analyze sales performance, profitability, product trends, and store-level performance across multiple locations.

The project focuses on transforming raw transactional data into meaningful business insights through data modeling, DAX calculations, and interactive visualizations. The dashboard provides a centralized view of key business metrics, enabling users to monitor sales trends, evaluate product performance, compare store results, and support data-driven decision-making.

---

## Project Objectives

- Analyze overall sales performance
- Monitor profitability and profit margins
- Identify top-performing products
- Compare store performance across different locations
- Track sales trends over time
- Evaluate category-level contribution
- Build an interactive and user-friendly dashboard

---

## Data Preparation

The dataset was imported into Power BI and transformed using Power Query Editor.

Key data preparation activities included:

- Data cleaning and validation
- Handling missing and inconsistent records
- Data type conversion
- Column formatting and renaming
- Creation of derived fields
- Building a Calendar Table for date-based analysis
- Optimizing the data model for reporting performance

---

## Data Modeling

A Star Schema data model was implemented to improve report performance and maintain data consistency.

### Fact Table

- Sales

### Dimension Tables

- Products
- Stores
- Inventory
- Calendar
- Locations

Relationships were created between fact and dimension tables to ensure accurate aggregations and filtering across visuals.

---

## DAX Functions Used

### Aggregation Functions

```DAX
SUM()
AVERAGE()
COUNT()
COUNTROWS()
MIN()
MAX()
DISTINCTCOUNT()
```

### Calculation Functions

```DAX
CALCULATE()
FILTER()
ALL()
DIVIDE()
IF()
SWITCH()
```

### Relationship Functions

```DAX
RELATED()
RELATEDTABLE()
```

### Context Functions

```DAX
VALUES()
SELECTEDVALUE()
HASONEVALUE()
```

### Ranking Functions

```DAX
RANKX()
TOPN()
```

### Date Functions

```DAX
YEAR()
MONTH()
FORMAT()
DATE()
TODAY()
```

### Time Intelligence Functions

```DAX
TOTALYTD()
DATESYTD()
DATEADD()
SAMEPERIODLASTYEAR()
```

---

## Measures Created

### Total Sales

```DAX
Total Sales =
SUM(Sales[Revenue])
```

### Total Cost

```DAX
Total Cost =
SUM(Sales[Cost])
```

### Total Profit

```DAX
Total Profit =
[Total Sales] - [Total Cost]
```

### Profit Margin %

```DAX
Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)
```

### Total Orders

```DAX
Total Orders =
COUNTROWS(Sales)
```

### Average Sales

```DAX
Average Sales =
AVERAGE(Sales[Revenue])
```

### Units Sold

```DAX
Units Sold =
SUM(Sales[Units])
```

---

## Dashboard Features

### KPI Cards

The dashboard includes KPI cards to provide a high-level overview of business performance.

- Total Sales
- Total Profit
- Profit Margin %
- Total Orders
- Units Sold

### Sales Trend Analysis

Line charts were created to analyze monthly and yearly sales trends, enabling users to identify seasonal patterns and business growth opportunities.

### Product Performance Analysis

Bar and column charts were used to evaluate product-level performance and identify top-selling products.

### Category Analysis

Interactive visuals were developed to understand category-wise sales and profit contribution.

### Store Performance Analysis

Store-level comparisons help identify high-performing and underperforming locations.

### Interactive Filtering

Slicers were added to allow dynamic analysis based on:

- Year
- Month
- Product Category
- Product Name
- Store
- Location

---

## Visualizations Used

- KPI Cards
- Line Charts
- Clustered Column Charts
- Bar Charts
- Donut Charts
- Tables
- Matrix Visuals
- Slicers

---

## Key Business Insights

The dashboard enables users to:

- Track overall business performance
- Identify top-performing products and categories
- Analyze sales trends over time
- Monitor profitability and profit margins
- Compare store performance across locations
- Discover revenue-driving products
- Support data-driven business decisions

---

## Skills Demonstrated

- Power BI Desktop
- Power Query
- Data Cleaning
- Data Transformation
- Data Modeling
- Star Schema Design
- Relationship Management
- DAX Development
- Time Intelligence Calculations
- KPI Creation
- Data Visualization
- Interactive Dashboard Design
- Business Intelligence Reporting

---

## Conclusion

This project demonstrates the complete Power BI development lifecycle, including data preparation, transformation, data modeling, DAX measure creation, KPI development, and interactive dashboard design.

The final dashboard provides meaningful insights into sales, profitability, product performance, and store operations while following Power BI and Business Intelligence best practices.

---

## Author

**Sakshi Raghuwanshi**

Programmer Analyst  
Power BI Developer | Data Analytics | Business Intelligence
