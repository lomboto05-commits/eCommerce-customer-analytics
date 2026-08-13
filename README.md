# E-Commerce Customer Analytics

## Project Overview

This project analyses an e-commerce dataset to understand customer spending behaviour, product performance, revenue trends, pricing patterns and discount behaviour.

The analysis was developed using Python and focuses on extracting practical business insights from transactional data.

The project demonstrates the use of data cleaning, exploratory data analysis, aggregation, statistical analysis and data visualisation to investigate an e-commerce dataset.

---

## Business Objectives

The analysis aims to answer questions such as:

- How much do customers typically spend?
- Which product categories generate the most revenue?
- How does revenue change over time?
- How do different discount levels relate to revenue and purchase volume?
- How are product prices distributed?
- What relationships exist between original price, discount and final price?
- How does pricing differ between product categories?
- Which customer value segments contribute the most revenue?

---

## Dataset

The dataset was sourced from **Kaggle** and contains **3,660 e-commerce transactions from 3,660 unique customers**.

The dataset contains the following key variables:

| Column | Description |
|---|---|
| `User_ID` | Customer identifier |
| `Product_ID` | Product identifier |
| `Category` | Product category |
| `Price (Rs.)` | Original product price |
| `Discount (%)` | Applied discount percentage |
| `Final_Price(Rs.)` | Price after discount |
| `Payment_Method` | Payment method used |
| `Purchase_Date` | Transaction date |

The dataset was prepared and updated for this analysis and is included in the repository as:

`ecommerce_dataset_updated.csv`

### Dataset Source

**Source:** Kaggle

> Note: The analysis uses the dataset as provided and does not claim that observed relationships represent causation.

Each customer appears once in the dataset, meaning repeat-purchase behaviour and customer retention cannot be directly evaluated from the available data.

---

## Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**
- **Git**
- **GitHub**

---

## Analysis Performed

### 1. Data Exploration

Initial exploration was performed to understand:

- Dataset structure
- Available variables
- Unique customers
- Unique products
- Product categories
- Payment methods
- Purchase dates
- Basic characteristics of the dataset

---

### 2. Customer Analysis

Customer-level analysis was performed to investigate:

- Total customer spending
- Average customer spending
- Median customer spending
- Minimum customer spending
- Maximum customer spending
- Customer purchase frequency
- Customer value segmentation

Key customer spending statistics:

| Metric | Value |
|---|---:|
| Average Customer Spend | Rs. 206.91 |
| Median Customer Spend | Rs. 199.19 |
| Minimum Customer Spend | Rs. 5.89 |
| Maximum Customer Spend | Rs. 496.82 |
| Unique Customers | 3,660 |

---

### 3. Customer Value Segmentation

Customers were divided into four value segments based on spending:

| Segment | Customers | Average Spend | Total Revenue |
|---|---:|---:|---:|
| Low Value | 915 | Rs. 54.73 | Rs. 50,071 |
| Mid-Low Value | 915 | Rs. 151.42 | Rs. 138,553 |
| Mid-High Value | 915 | Rs. 248.85 | Rs. 227,693 |
| High Value | 915 | Rs. 372.63 | Rs. 340,961 |

The **High Value** customer segment generated the largest amount of revenue despite containing the same number of customers as each of the other segments.

---

### 4. Product & Category Analysis

Product categories were analysed using:

- Number of purchases
- Total revenue
- Average purchase value
- Average product price
- Average discount
- Average final selling price

The analysis identified differences in revenue performance and pricing between product categories.

---

### 5. Revenue Analysis

Revenue trends were analysed over time to identify changes in monthly performance.

Monthly revenue was compared to identify periods of stronger and weaker performance.

The available data showed:

- **October** as the highest-revenue month at approximately **Rs. 76,035**
- **November** as the lowest-revenue month in the available data at approximately **Rs. 51,915**

Revenue was also compared across product categories and customer value segments.

---

### 6. Payment Method Analysis

Payment methods were compared based on:

- Number of purchases
- Total revenue
- Average purchase value

The available payment methods were:

- Credit Card
- UPI
- Debit Card
- Net Banking
- Cash on Delivery

Credit Card transactions generated the highest total revenue in the dataset.

---

### 7. Discount Analysis

Discount behaviour was analysed using:

- Revenue by discount level
- Purchase volume by discount level
- Average purchase value
- Discount efficiency
- Average discount by category

The analysis showed that revenue generally decreased as discount levels increased.

Purchase volumes remained relatively stable across many discount levels, suggesting that larger discounts did not necessarily result in proportionally higher purchase volumes.

---

### 8. Pricing Analysis

Product pricing was analysed using:

- Original price distribution
- Average price by category
- Average final price by category
- Relationship between original price and final price
- Relationship between discount and final price

Product prices were relatively evenly distributed across the available price range of approximately **Rs. 0–500**.

---

### 9. Correlation Analysis

A correlation matrix was used to examine relationships between:

- Original price
- Discount percentage
- Final price

The analysis identified:

- A very strong positive relationship between original price and final price.
- A negative relationship between discount percentage and final price.
- A very weak relationship between original price and discount percentage.

Correlation indicates the strength of an observed relationship but does not establish causation.

---

## Key Findings

### Customer Insights

- The dataset contains **3,660 unique customers**.
- Each customer appears only once.
- Average customer spend was approximately **Rs. 206.91**.
- Median customer spend was approximately **Rs. 199.19**.
- Customer spending ranged from approximately **Rs. 5.89 to Rs. 496.82**.
- High-value customers generated substantially more revenue than lower-value segments.

### Category Insights

- **Clothing** generated the highest category revenue at approximately **Rs. 115,315**.
- **Electronics** generated the lowest category revenue at approximately **Rs. 100,462**.
- Average product prices were relatively consistent across categories.
- Clothing had the highest average original price at approximately **Rs. 263**.
- Clothing also had the highest average final selling price.

### Revenue Insights

- Monthly revenue fluctuated throughout the available 2024 period.
- October recorded the highest monthly revenue.
- November recorded the lowest monthly revenue in the available data.
- Further investigation would be required to determine the reasons behind monthly fluctuations.

### Discount Insights

- Revenue generally decreased as discount levels increased.
- Purchase volumes were relatively stable across most discount levels.
- Home & Kitchen had the highest average discount at approximately **19.6%**.
- Clothing had the lowest average discount at approximately **17.9%**.
- Larger discounts were associated with lower final selling prices and lower total revenue.

### Pricing Insights

- Original price and final price showed a **very strong positive correlation**.
- Discount percentage had a negative relationship with final price.
- Product prices were relatively evenly distributed across the available price range.

---

## Business Recommendations

Based on the analysis, several potential business actions can be considered.

### 1. Focus on High-Value Customers

The High Value customer segment generates significantly more revenue per customer.

Businesses could consider targeted loyalty programmes, personalised offers and retention strategies for high-value customers.

### 2. Review Discount Strategy

Higher discount levels were associated with lower total revenue.

Rather than relying heavily on large discounts, businesses could investigate targeted promotions that encourage purchases while protecting average selling prices.

### 3. Investigate Clothing Performance

Clothing generated the highest category revenue and had the highest average product price.

Further analysis could investigate which individual clothing products are responsible for this performance.

### 4. Investigate Revenue Declines

The decline in revenue observed in November could be investigated further.

Potential factors could include:

- Seasonal demand
- Product availability
- Pricing changes
- Promotional activity
- Changes in customer behaviour

Additional data would be required to determine the actual cause.

---

## Limitations

There are several limitations to the analysis.

- Each customer appears only once, so repeat-purchase behaviour cannot be evaluated.
- Customer retention and customer lifetime value cannot be calculated from the available transactions.
- The dataset does not contain detailed customer demographic information.
- The dataset does not provide detailed product descriptions.
- Correlation does not imply causation.
- The available purchase dates cover only part of 2024.
- The analysis focuses on the variables available in the dataset.

---

## Project Structure

```text
eCommerce-customer-analytics/
│
├── ecommerce_customer_analytics.ipynb
├── ecommerce_dataset_updated.csv
├── .gitignore
└── README.md
