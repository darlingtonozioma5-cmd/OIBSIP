# Customer Segmentation Analysis

**Oasis Infobyte Internship – Data Analytics | Level 1, Task 2**

## 1. Project Overview

This project focuses on customer segmentation using transactional retail data. The objective is to identify different customer groups based on their purchasing behaviour and provide business insights that can support targeted marketing strategies and customer retention.

The analysis uses Recency, Frequency and Monetary (RFM) analysis combined with K-Means clustering.

## 2. Dataset Description

The project uses the UCI Online Retail dataset, which contains transactional records from a UK-based online retail business.

**Dataset source:** [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

The dataset includes:
- Invoice numbers
- Product descriptions
- Quantities purchased
- Invoice dates
- Unit prices
- Customer IDs
- Countries

## 3. Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## 4. Data Preparation

The dataset was inspected and prepared before performing customer segmentation.

The preparation process included:
- Inspecting the dataset structure and data types.
- Removing duplicate records.
- Handling missing customer and transaction information.
- Removing cancelled invoices and invalid transactions.
- Converting transaction dates and numerical columns to appropriate formats.
- Calculating transaction revenue.

## 5. Analysis and Methodology

### RFM Analysis

Three key customer behaviour metrics were calculated:

- **Recency:** Number of days since a customer's most recent purchase.
- **Frequency:** Number of distinct invoices associated with a customer.
- **Monetary:** Total historical spending by a customer.

Average Purchase Value and purchase frequency were also examined.

### Feature Scaling

The RFM features were log-transformed and standardised using StandardScaler to prepare them for clustering.

### K-Means Clustering

K-Means clustering was used to group customers with similar purchasing behaviour.

The Elbow Method was used to examine suitable cluster counts. The resulting clusters were evaluated and profiled using their RFM characteristics.

### Visualisations

The project includes:
- Elbow Method chart.
- Customer count per cluster.
- Recency versus Frequency scatter plot.
- Frequency versus Monetary scatter plot.
- RFM distribution charts.
- Cluster profile visualisations.

## 6. Key Findings

The analysis examined customer purchasing behaviour using Recency, Frequency and Monetary metrics.

The following findings are to be completed using the actual clustering results:

- Total number of customers analysed:4338
- Number of customer segments created:4
- Largest customer segment: Cluster 1, with 1622 customers
- Highest-value customer segment: Cluster 0
- Least recently active segment: Cluster 1
- Most frequent purchasing segment: Cluster 0

## 7. Business Recommendations

Based on the customer segmentation results, the following strategies can be considered:

1. **Customer Loyalty:** Introduce loyalty rewards and exclusive offers for customers with high purchase frequency and monetary value.

2. **Customer Retention:** Develop targeted retention campaigns for valuable customers who have not purchased recently.

3. **Customer Re-engagement:** Use personalised promotions and product recommendations to encourage inactive customers to return.

4. **Repeat Purchases:** Offer incentives to customers with low purchase frequency to encourage more regular transactions.

5. **Targeted Marketing:** Develop different marketing campaigns for each customer segment instead of applying the same strategy to all customers.

## 8. Project Outputs

The project repository contains:
- Python analysis notebook.
- Customer segmentation results CSV.
- Cluster profile summary.
- Elbow Method visualisation.
- Customer distribution chart.
- RFM scatter plots.
- Other analysis visualisations.

## 9. Conclusion

This project demonstrates how RFM analysis and K-Means clustering can be used to identify customer groups based on purchasing behaviour.

The resulting segmentation provides a foundation for targeted marketing, customer retention and improved customer relationship management.
