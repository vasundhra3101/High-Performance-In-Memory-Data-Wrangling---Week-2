# High-Performance In-Memory Data Wrangling - Week 2

## Project Overview

This project demonstrates high-performance data wrangling using the **R programming language** and the **data.table** package. A sales transaction dataset is generated, imported, cleaned, transformed, analyzed, and visualized to produce business insights.

The project showcases efficient in-memory data processing techniques, including indexing, grouping, aggregation, and visualization.

---

## Objectives

- Generate a sales transaction dataset.
- Import data using `fread()`.
- Explore and summarize the dataset.
- Clean and validate the data.
- Perform data manipulation using `data.table`.
- Apply in-place column updates.
- Use indexing with `setkey()`.
- Perform grouping and aggregation.
- Generate business reports.
- Create visualizations for data analysis.

---

## Technologies Used

- R Programming
- data.table
- ggplot2

---

## Project Structure

```
High-Performance-DataWrangling-Week2/
│── README.md
│── Week2_Report.pdf
│── sales_transactions.csv
│── high_performance_data_wrangling.R
└── Output/
    ├── customer_summary.csv
    ├── product_summary.csv
    ├── city_summary.csv
    ├── category_summary.csv
    ├── city_transactions.png
    ├── category_revenue.png
    ├── top_customers.png
    └── payment_distribution.png
```

---

## Dataset Information

The generated dataset contains **5,000 sales transaction records** with the following fields:

- Transaction_ID
- Customer_ID
- Product_ID
- City
- Category
- Quantity
- Price
- Payment_Method
- Date
- Total_Amount

Additional columns created during analysis:

- Discount
- Net_Amount
- Month

---

## Project Workflow

### Part 1 – Generate Dataset

- Generate 5,000 random sales transactions.
- Store the dataset as `sales_transactions.csv`.

### Part 2 – Import Dataset

- Import data using `fread()`.
- Verify the dataset structure.

### Part 3 – Explore Dataset

- Display sample records.
- View summary statistics.
- Check missing values.
- Detect duplicate records.

### Part 4 – Data Cleaning

- Remove duplicate rows.
- Remove missing values.
- Validate cleaned dataset.

### Part 5 – Data Manipulation

- Calculate Discount.
- Calculate Net Amount.
- Extract Month from Date.

### Part 6 – In-place Column Updates

- Update columns efficiently using the `:=` operator.

### Part 7 – Index Keying

- Improve query performance using `setkey()`.

### Part 8 – Grouping and Aggregation

Generate summary reports:

- Customer Summary
- Product Summary
- City Summary
- Category Summary

### Part 9 – Business Reports

Generate key business insights such as:

- Total Revenue
- Total Transactions
- Best Performing City
- Best Product Category
- Top Customer
- Most Used Payment Method

### Part 10 – Visualization

Generate the following charts:

- City Transactions
- Category Revenue
- Top Customers
- Payment Distribution

---

## Output Files

### CSV Reports

- customer_summary.csv
- product_summary.csv
- city_summary.csv
- category_summary.csv

### Visualizations

- city_transactions.png
- category_revenue.png
- top_customers.png
- payment_distribution.png

---

## How to Run

1. Install the required packages:

```r
install.packages("data.table")
install.packages("ggplot2")
```

2. Open the project in RStudio.

3. Set the working directory.

```r
setwd("Project Folder")
```

4. Run the script:

```r
source("high_performance_data_wrangling.R")
```

5. Output files will be generated inside the **Output** folder.

---

## Learning Outcomes

Through this project, the following concepts were implemented:

- High-performance data processing
- Efficient in-memory data manipulation
- Data cleaning
- Aggregation
- Business analytics
- Data visualization
- Report generation
- Working with `data.table`

---

##Category Revenue

<img width="2100" height="1500" alt="category_revenue" src="https://github.com/user-attachments/assets/9b02b715-c887-44b1-b592-a8413e20c576" />

##City Transactions

<img width="2100" height="1500" alt="category_revenue" src="https://github.com/user-attachments/assets/f89c9091-83bf-4ea3-b577-54e4ce9fce33" />

##Payment Distribution

<img width="2100" height="1500" alt="payment_distribution" src="https://github.com/user-attachments/assets/8f986c03-cbb3-4ca0-804e-753c39d15bb6" />

##Top Customers

<img width="2400" height="1500" alt="top_customers" src="https://github.com/user-attachments/assets/20c896d9-a2f8-40d5-a20d-915ba090e76d" />
