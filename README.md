# Customer Segmentation Using K-Means

## Overview

This project explores customer segmentation for a luxury clothing brand using unsupervised machine learning.

Customers are segmented based on four characteristics:

- Income
- Age
- Days since last purchase
- Annual spending

The objective is to identify distinct customer profiles and translate the resulting clusters into actionable marketing strategies.

## Notebook

The complete analysis is available in [`customer_segmentation.ipynb`](customer_segmentation.ipynb).

## Methodology

The analysis follows these main steps:

1. Data exploration and preprocessing
2. Feature standardization
3. PCA for two-dimensional visualization
4. K-means clustering using the four standardized features
5. Cluster evaluation using the elbow method and silhouette score
6. Customer profiling and segment interpretation
7. Marketing recommendations

Both the elbow method and silhouette score support a **five-cluster solution**.

PCA is used only for visualization; the final clustering is performed using all four standardized variables.

## Customer Segments

The analysis identifies five customer profiles:

| Segment | Main characteristics |
|---|---|
| Young High-Income Low Spenders | High income, young, relatively recent activity, low annual spending |
| Mature High Spenders - Inactive | Mature customers, high spending, low recent activity |
| Young Low-Value Inactive Customers | Young customers, lower spending and low recent activity |
| High-Income High-Value Customers - Inactive | High income and spending, but low recent activity |
| Active High Spenders | High spending and relatively recent purchasing activity |

## Business Insights

The segmentation suggests several potential marketing strategies:

- **Retention:** maintain engagement among active high spenders through loyalty initiatives and personalized recommendations.
- **Reactivation:** target historically valuable but inactive customers with personalized campaigns.
- **Cross-selling:** encourage young high-income customers with relatively low spending to explore additional or higher-value products.
- **Marketing efficiency:** use lower-cost automated campaigns for currently lower-value and inactive customers.

These recommendations should be considered hypotheses to test rather than demonstrated causal effects.

## Tools

- Python
- pandas
- scikit-learn
- matplotlib
- Jupyter Notebook

## Limitations

The segmentation is based on four customer characteristics and provides a descriptive view of customer behavior.

Additional variables such as purchase frequency, product preferences, acquisition channels or campaign responses could improve the segmentation and enable more precise targeting.

## Project Origin

This project was initially based on a clustering exercise from *Data Science for Marketing Analytics*.

The original exercise was extended and reworked to focus on model evaluation, customer profiling, business interpretation and actionable marketing recommendations.
