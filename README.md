# Amazon Sales Analysis Dashboard (Power BI)

## Project Overview

The Amazon Product Analysis Dashboard is an interactive Power BI report developed to analyze product pricing, discounts, ratings, reviews, and category performance. The dashboard provides a comprehensive view of Amazon product data, helping identify top-performing categories, pricing trends, and customer engagement patterns.

Through data cleaning, transformation, and visualization, the dashboard converts raw product data into actionable business insights.

---

## Objective

The objective of this project is to analyze Amazon product data and uncover trends related to product pricing, discounts, customer ratings, and reviews.

This project demonstrates the ability to:

* Clean and transform raw data using Power Query
* Build data models and calculated fields using DAX
* Create interactive dashboards in Power BI
* Analyze product performance across categories
* Generate meaningful business insights through data visualization

---

## Dataset Information

The dataset contains product-related information such as:

| Column Name         | Description                        |
| ------------------- | ---------------------------------- |
| Product ID          | Unique identifier for each product |
| Product Name        | Name of the product                |
| Category            | Product category                   |
| Actual Price        | Original product price             |
| Discounted Price    | Selling price after discount       |
| Discount Percentage | Discount offered on the product    |
| Rating              | Average customer rating            |
| Rating Count        | Number of customer ratings         |
| Review Content      | Customer reviews                   |

---

## Data Preparation

The following data cleaning and transformation steps were performed:

* Removed unnecessary columns
* Cleaned price-related fields
* Converted data types into numeric formats
* Cleaned discount percentage values
* Handled missing and invalid records
* Created Price Range categories
* Created Discount Amount calculations
* Built DAX measures for KPI analysis

---

## Dashboard Features

### Key Performance Indicators (KPIs)

* Average Discount: **47.7%**
* Average Rating: **4.10**
* Total Products: **1K**
* Average Selling Price: **₹3K**
* Total Reviews: **27M**

---

### Visualizations Used

| Visualization          | Description                                     |
| ---------------------- | ----------------------------------------------- |
| KPI Cards              | Product performance summary                     |
| Clustered Column Chart | Actual Price vs Discounted Price                |
| Horizontal Bar Chart   | Top Categories by Products                      |
| Area Chart             | Product Distribution Analysis                   |
| Bar Chart              | Products by Price Range                         |
| Scatter Chart          | Rating vs Price Analysis                        |
| Slicers                | Category, Product Name, Price Range, Discount % |

---

## Key Insights

* Electronics is the largest product category in the dataset.
* Computers & Accessories and Home & Kitchen also contribute significantly to product volume.
* Products are heavily concentrated in the lower and mid-price ranges.
* Average customer rating remains above 4.0, indicating generally positive customer satisfaction.
* Most products receive substantial discounts, with an average discount of 47.7%.
* The Rating vs Price analysis shows that higher prices do not always result in higher ratings.
* Customer engagement is concentrated around selected high-performing products.

---

## DAX Measures Used

```DAX
Total Products = DISTINCTCOUNT(Amazon[product_id])

Average Rating = AVERAGE(Amazon[rating])

Average Discount = AVERAGE(Amazon[discount_percentage])

Total Reviews = SUM(Amazon[rating_count])

Average Selling Price = AVERAGE(Amazon[discounted_price])
```

---

## Dashboard Design Highlights

* Dark-themed professional dashboard layout
* Interactive slicers for dynamic filtering
* KPI-focused design for quick decision-making
* Consistent visual styling and formatting
* User-friendly navigation and storytelling

---

## Tools & Technologies Used

* Microsoft Power BI Desktop
* Power Query
* DAX (Data Analysis Expressions)
* Microsoft Excel

---

## Project Structure

```text
  Amazon-Product-Analysis-Dashboard

| Amazon_Product_Analysis.pbix
| Dashboard_Screenshot.png
| README.md
| Amazon_Dataset.xlsx
| amazon.csv
```

---

## Dashboard Preview

https://github.com/bhivanshushrivastava/Amazon_Sales_Data_powerbi_dashboard/blob/main/Amazon_sales_data_pnd.png

---

## Project Summary

I built this Power BI dashboard to analyze Amazon product ratings, pricing, discounts, reviews, and category performance. Using Power Query for data transformation and DAX for calculations, I created an interactive dashboard that helps identify top-performing categories, pricing patterns, customer engagement trends, and product performance insights. The project demonstrates end-to-end data analytics skills, including data cleaning, modeling, visualization, and business intelligence reporting.
