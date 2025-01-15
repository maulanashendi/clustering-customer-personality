# Customer Personality Analysis and Clustering

This repository contains the implementation and analysis of customer personality segmentation using clustering techniques. The project is aimed at understanding customer characteristics to improve marketing strategies and optimize resource allocation.

## About the Data

The dataset provides information about customer demographics, spending habits, and interactions with campaigns. It is sourced from Kaggle:

- Dataset: [Customer Personality Analysis](https://www.kaggle.com/imakash3011/customer-personality-analysis)
- Notebook: [GitHub Repository](https://github.com/mpsmaul/my-project/tree/master/Customer%20Personality)

### Dataset Overview
The dataset contains:
- Customer demographics (age, income, etc.)
- Spending habits on various product categories (wine, fruits, meat, fish, etc.)
- Campaign participation details

## Goals

- Predict the characteristics of consumer purchasing habits.
- Reduce marketing costs by at least 30%.
- Enhance marketing ROI through targeted strategies.

## Methodology

### Clustering Technique
The project employs **K-Means Clustering** for segmenting customers into distinct groups based on their behaviors and characteristics. Key steps include:

1. **Data Preprocessing**
   - Scaling using `StandardScaler`.
   - Dimensionality reduction using PCA.

2. **Modeling**
   - Number of clusters: 4

### Clusters Overview

1. **Alpha Cyan**
   - Size: 826 (37%)
   - Median Age: 55 years
   - Average Income: $68,774
   - Preferences: Loves all products; shops frequently offline and online.

2. **Beta Red**
   - Size: 324 (14.4%)
   - Median Age: 55 years
   - Average Income: $51,550
   - Preferences: Prefers wine; moderate spending; highly active in campaigns.

3. **Teta Orange**
   - Size: 112 (5%)
   - Median Age: 47 years
   - Average Income: $82,092
   - Preferences: Buys all products in bulk; active offline and moderately active online.

4. **Delta Purple**
   - Size: 976 (43.6%)
   - Median Age: 48 years
   - Average Income: $33,729
   - Preferences: Low spending; minimal participation in campaigns.

## Results and Recommendations

- Enhance services for offline and online platforms to cater to the majority preference.
- Offer product-specific campaigns:
  - **Alpha Cyan** & **Teta Orange**: All products.
  - **Beta Red**: Focus on wine products.
- Campaign 4 and 6 are the most effective based on historical data.

### ROI Analysis

Using a guesstimate method to evaluate potential ROI improvements:

- **Before Clustering**:
  $$ROI = \frac{500,000 - 200,000}{200,000} = 1.5$$

- **After Clustering**:
  $$ROI = \frac{500,000 - 140,000}{140,000} = 2.5$$

## File Structure

- **`marketing_campaign.csv`**: Dataset used for analysis.
- **`Customer Personality Analysis.ipynb`**: Jupyter Notebook containing the clustering implementation and visualizations.
- **`Clustering Customers.pdf`**: Detailed report of the analysis and findings.

## Tools and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib/Seaborn
