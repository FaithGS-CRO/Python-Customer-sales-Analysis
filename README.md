# Customer Sales Analysis

## Project Overview

This project analyzes customer behaviour, spending patterns, and conversion on an online shopping website using customer data, website session, and transaction data.

The goal is to identify patterns and trends that provide insights into customer purchasing behaviour, sales performance, and areas of business opportunity.

## Business Questions

* Which countries generate the highest sales?
* Which product categories generate the highest sales?
* How do sales change across years?
* What happened to sales during the decline in 2021?
* What are the spending patterns across different countries and product categories?
* Is there a relationship between time spent on the website and purchase value?
* Which acquisition channels have higher conversion?

## Dataset

The analysis uses three datasets:

### Customers

Contains customer information including:

* Customer ID
* Gender
* Country
* Acquisition channel

### Transactions

Contains purchase information including:

* Customer ID
* Purchase date
* Purchase value
* Product category

### Web Sessions

Contains website behaviour including:

* Customer ID
* Pages viewed
* Time spent on site
* Conversion status

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

## Analysis Approach

The analysis followed these steps:

1. Explored the datasets to understand their structure and variables.
2. Examined customer, transaction, and website session data.
3. Merged datasets using `customer_id` where required.
4. Analyzed sales by country, product category, and year.
5. Examined customer spending patterns.
6. Analyzed website behaviour and conversion.
7. Investigated changes in sales over time.
8. Used visualizations to identify patterns and trends.

## Key Findings

**1** Analysis: Examined the relationship between time spent on site and purchase value, and compared time spent by converted and non-converted users.

Insight: There is almost no correlation between time spent and purchase value (r = 0.00016). Converted users spent slightly longer on average (301.05s vs. 294.96s).

Recommendation: Improve navigation and simplify the path to purchase so customers can complete purchases efficiently.

**2** Analysis: Compared purchase value and average customer age across product categories.

Key Findings:

Electronics had the highest sales, while Toys had the lowest.
Overall average customer age was 43 years.
Average age across categories was very similar (43.19–43.68 years).

Insight: Customer age is unlikely to be a major driver of differences in product sales.

Recommendation: Investigate pricing, demand, availability, and customer preferences to understand the sales differences.

**3** Analysis: Calculated total sales by year, country, and product category to identify key sales drivers.

Insights:

2022 recorded the highest total sales.
France contributed significantly to overall sales, driven largely by electronics.
Electronics had the highest total purchase value among product categories.

Recommendation: Prioritize electronics in high-performing markets such as France while exploring ways to strengthen other categories. Further analysis of transaction volume and average purchase value could help explain the sales differences.

**4** Analysis: Compared sales across years and countries to identify factors contributing to the 2021 decline.

Insight: Sales declined in 2021, largely due to lower sales from France, but recovered in 2022. This shows the impact a decline in a major market can have on overall performance.

Recommendation: Reduce reliance on a single high-performing market by strengthening sales across other countries and product categories.

**5** Analysis: Compared conversion rates across acquisition channels to identify which channels generated the highest proportion of converted customers.

Insight: Social Media recorded the highest conversion rate among the channels analyzed, making it the strongest channel for converting visitors into customers.

Recommendation: Consider increasing focus on Social Media while monitoring its performance and conversion efficiency.

### The project includes visualizations for:

* Sales by year
* Sales by country
* Sales by product category
* Sales by country and product category
* Purchase value

# Business Insights

The analysis highlights several areas that may require further investigation, particularly the decline in sales during 2021.

Potential areas for further analysis include:

* Investigating the factors behind the 2021 sales decline, particularly the decline in France.
* Examining transaction volume and average purchase value to understand sales differences.
* Investigating why electronics significantly outperformed other product categories.
* Exploring factors beyond age that may influence product performance.
* Investigating factors associated with customer conversion and acquisition channels.
* Examining customer purchasing behaviour across countries and product categories.

Limitations
The available data does not explain the underlying reasons for changes in sales.
Correlation does not necessarily imply causation.
Website session data may not capture all factors influencing customer purchasing decisions.
Additional business and customer data would be needed to determine the exact causes of changes in sales.

## Project Structure
Customer-Sales-Analysis/
│
├── customer_sales_analysis.ipynb
├── README.md
└── data/
    ├── customers.csv
    ├── transactions.csv
    └── web_sessions.csv
```

## Conclusion

This analysis provides an overview of customer purchasing behaviour and sales performance across countries, product categories, acquisition channels, and years.

The analysis identified key sales trends, including the 2021 sales decline, the strong performance of electronics, and differences in customer conversion across acquisition channels. It also demonstrates how data analysis can be used to identify trends and generate business insights from transactional and website data.