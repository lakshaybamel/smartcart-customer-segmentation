# SmartCart Customer Segmentation using Machine Learning

## Project Overview

Customer segmentation is a key strategy for modern e-commerce platforms. Instead of treating all customers the same, businesses can group customers based on their behavior and target them with personalized marketing strategies.

In this project, we build a **Customer Segmentation System** for SmartCart, an e-commerce platform that has collected detailed customer data including demographics, purchasing behavior, and website activity.

Using **unsupervised machine learning techniques**, the project identifies meaningful customer groups based on behavioral patterns. These segments can help businesses improve marketing strategies, customer engagement, and revenue generation.

---

## Problem Statement

SmartCart currently applies a **generic marketing strategy to all customers**, which leads to several inefficiencies:

* Ineffective targeting of high-value customers
* Missed opportunities for customer retention
* Difficulty identifying churn-prone users
* Poor allocation of marketing resources

To address this issue, we apply **clustering algorithms** to group customers with similar behaviors into distinct segments.

---

## Dataset Description

The dataset contains **2240 customer records** and **22 attributes** describing customer demographics, purchasing behavior, and engagement activity.

### Customer Demographics

* Year_Birth
* Education
* Marital_Status
* Income
* Kidhome
* Teenhome
* Dt_Customer

### Purchase Behavior (Amount Spent)

* MntWines
* MntFruits
* MntMeatProducts
* MntFishProducts
* MntSweetProducts
* MntGoldProds

### Purchase Behavior (Frequency)

* NumDealsPurchases
* NumWebPurchases
* NumCatalogPurchases
* NumStorePurchases
* NumWebVisitsMonth

### Customer Engagement

* Recency
* Complain

---

## Machine Learning Pipeline

The project follows a complete machine learning workflow:

1. Data Exploration
2. Data Preprocessing
3. Feature Engineering
4. Outlier Detection
5. Feature Scaling
6. Dimensionality Reduction using PCA
7. Determining optimal clusters using:

   * Elbow Method
   * Silhouette Score
8. Customer segmentation using clustering algorithms:

   * K-Means Clustering
   * Agglomerative Hierarchical Clustering
9. Cluster Visualization and Analysis
10. Business Insights and Recommendations

---

## Feature Engineering

Several new features were created to better capture customer behavior:

* **Age** – calculated from birth year
* **Customer Tenure** – time since customer joined
* **Total Spending** – overall spending across product categories
* **Total Children** – number of children in household
* **Living_With** – simplified marital status

These engineered features improve the quality of customer segmentation.

---

## Determining Optimal Clusters

To determine the best number of clusters, we used:

* **Elbow Method**
* **Silhouette Score**

Both methods suggested that **four clusters** provide a meaningful segmentation of the customer base.

---

## Clustering Algorithms Used

### K-Means Clustering

Primary clustering method used for segmentation.

Advantages:

* Fast and scalable
* Produces balanced clusters
* Commonly used in customer segmentation problems

### Agglomerative Hierarchical Clustering

Used as a comparison method to evaluate clustering robustness.

---

## Cluster Visualization

To visualize high-dimensional customer data, we applied **Principal Component Analysis (PCA)** and plotted clusters in 2D and 3D space.

These visualizations help illustrate how customers are grouped based on behavioral similarity.

---

## Customer Segments Identified

The clustering model identified **four distinct customer segments**:

### Cluster 0 – Low Spending Couples

Customers with moderate income but low spending. They frequently browse the website but rarely make purchases.

### Cluster 1 – High Value Customers

Customers with the highest income and spending levels. They represent the most valuable segment for the business.

### Cluster 2 – Regular Customers

Customers with moderate income and consistent purchasing behavior.

### Cluster 3 – Low Spending Singles

Customers with lower spending levels and moderate website activity.

---

## Business Insights

Customer segmentation enables SmartCart to move from **generic marketing strategies** to **targeted customer engagement**.

Potential strategies include:

* Loyalty programs for high-value customers
* Discount campaigns for price-sensitive customers
* Personalized product recommendations
* Targeted promotions for frequent website visitors

These insights can help improve **customer retention and marketing efficiency**.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Kneed

---

## How to Run the Project

Clone the repository:

```bash
git clone https://github.com/lakshaybamel/smartcart-customer-segmentation.git
cd smartcart-customer-segmentation
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook smartcart_clustering.ipynb
```

---

## Project Structure

```
smartcart-customer-segmentation
│
├── smartcart_clustering.ipynb
├── smartcart_customers.csv
├── requirements.txt
└── README.md
```

---

## Conclusion

This project demonstrates how **unsupervised machine learning techniques** can be used to discover hidden patterns in customer behavior.

By segmenting customers into meaningful groups, businesses can make **data-driven marketing decisions**, improve customer satisfaction, and increase revenue.
