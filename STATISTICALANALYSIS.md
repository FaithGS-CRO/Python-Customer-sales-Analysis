# Customer sales Statistical Analysis

## Project Overview

This project uses statistical analysis to investigate customer behaviour and determine whether observed differences and relationships in the data are statistically significant.

The analysis builds on the customer sales analysis by applying statistical tests to answer specific business questions and distinguish between patterns that may be meaningful and those that may simply occur by chance.

## Business Questions

* Do customers from different countries differ significantly in their purchase values?
* Do discounted and non-discounted transactions have significantly different purchase values?
* Does loyalty tier have a significant relationship with purchase value?
* Is there a relationship between pages viewed and purchase value?
* Is a statistically significant relationship meaningful from a business perspective?
* Are customer characteristics associated with customer behaviour?

## Statistical Tests Used

### Independent T-Test

Used to compare the average purchase value between two independent groups.

Examples:

* Discounted vs. non-discounted transactions
* Customers from different countries

### ANOVA

Used to compare average purchase values across more than two groups.

Example:

* Gold, Silver, Bronze, and None loyalty tiers

### Pearson Correlation

Used to measure the strength and direction of the relationship between two numerical variables.

Example:

* Pages viewed vs. purchase value
* Time spent on site vs. purchase value

### Chi-Square Test

Used to determine whether there is a statistically significant association between two categorical variables.

## Key Findings

### 1. Discounted vs. Non-Discounted Transactions

An independent t-test was used to compare purchase values between discounted and non-discounted transactions.

The difference was not statistically significant (p = 0.689).

The box plot also showed very similar purchase value distributions between the two groups.

**Business Interpretation:** There is not enough evidence to suggest that using a discount resulted in different purchase values in this dataset.

### 2. Loyalty Tier vs. Purchase Value

ANOVA was used to compare purchase values across Gold, Silver, Bronze, and None loyalty tiers.

The result was not statistically significant (F = 1.19, p = 0.312).

**Business Interpretation:** Customers in different loyalty tiers did not show significantly different purchase values. This suggests that purchase value alone may not be enough to evaluate the effectiveness of the loyalty programme. 

### 3. Pages Viewed vs. Purchase Value

Pearson correlation was used to examine the relationship between pages viewed and purchase value.

The result showed a statistically significant relationship (r = -0.004, p = 0.044). However, the correlation was extremely weak and very close to zero.

**Business Interpretation:** Although the relationship was statistically significant, the effect was too small to be practically meaningful. This demonstrates that statistical significance does not necessarily mean business importance.

### 4. Chi-Square Analysis

A Chi-square test was used to investigate whether there was a statistically significant association between device type and conversion

The test produced a chi-square statistic of 1.150 and a p-value of 0.563.

**Business Interpretation** There is no statistically significant association between device type and conversion (χ² = 1.150, p = 0.563)

## Statistical Significance vs. Business Importance

Statistical Significance vs. Business Importance

One of the key lessons from this analysis is that statistical significance does not automatically mean business significance.

A statistically significant result indicates that an observed relationship or difference is unlikely to be due to random chance. However, the strength and size of the effect also matter.

For Business Question 9, I analysed the relationship between pages viewed and purchase value using a Pearson correlation test. The result showed a correlation of -0.004 with a p-value of 0.044.

Since the p-value is below 0.05, the relationship is statistically significant. However, the correlation is almost zero, meaning the relationship is extremely weak and unlikely to have meaningful business impact.

This demonstrates that a result can be statistically significant without being practically or commercially important.

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* SciPy
* Jupyter Notebook

## Analysis Workflow

1. Cleaned and prepared the customer data.
2. Selected relevant variables for each statistical test.
3. Divided customers or transactions into appropriate groups.
4. Applied the relevant statistical test.
5. Interpreted the test statistic and p-value.
6. Used visualizations to support the statistical findings.
7. Considered the practical business meaning of each result.

## Project Structure

```text
Customer-Sales-Analysis/
│
├── customer_sales_analysis.ipynb
├── customer_statistical_analysis.ipynb
├── README.md
├── statistical_analysis_README.md
├── requirements.txt
│
└── data/
    ├── customers.csv
    ├── transactions.csv
    ├── web_sessions.csv
    
```

## Conclusion

The statistical analysis provided a deeper understanding of customer behaviour by testing whether observed differences and relationships were statistically significant.

While some relationships were statistically significant, their practical business impact was not always meaningful. This highlights the importance of combining statistical analysis with business context when interpreting data and making decisions.
