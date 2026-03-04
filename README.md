# 🛒 SmartCart Customer Segmentation using Machine Learning

## 📌 Project Overview

Customer segmentation is a key strategy for modern e-commerce platforms. Instead of treating all customers the same, businesses can group customers based on their behavior and target them with personalized marketing strategies.

In this project, we build a **Customer Segmentation System** for SmartCart using **unsupervised machine learning techniques**. By analyzing customer demographics, purchasing behavior, and engagement patterns, we identify meaningful customer groups that can help improve marketing strategies and customer engagement.

---

## 🚨 Problem Statement

SmartCart currently applies **generic marketing strategies to all customers**, which leads to several challenges:

* Inefficient marketing campaigns
* Difficulty identifying **high-value customers**
* Inability to detect **low engagement or churn-risk users**
* Poor targeting of promotions and offers

To solve this, we apply **customer segmentation using clustering algorithms** to group customers with similar behaviors.

---

## 📊 Dataset Description

The dataset contains **2240 customer records** with **22 attributes** related to demographics, purchasing behavior, and website activity.

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

## ⚙️ Machine Learning Pipeline

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

## 🧠 Clustering Algorithms Used

### 🔹 K-Means Clustering

Primary algorithm used for customer segmentation.

Advantages:

* Efficient for large datasets
* Produces balanced clusters
* Widely used in customer segmentation problems

### 🔹 Agglomerative Hierarchical Clustering

Used as a comparison method to evaluate clustering robustness.

---

## 📉 Determining Optimal Clusters

To determine the optimal number of clusters, we used:

* **Elbow Method**
* **Silhouette Score**

Both techniques suggested that **4 clusters** provide meaningful segmentation of the customer base.

---

## 📊 Cluster Visualization

Since the dataset contains many features, **Principal Component Analysis (PCA)** was applied to reduce dimensionality and visualize clusters in **2D and 3D space**.

This helps understand how customers are grouped based on behavioral similarity.

---

## 💡 Customer Segments Identified

The clustering model identified **four distinct customer groups**:

### Cluster 0 – Low Spending Couples

Customers with moderate income but relatively low spending levels. They frequently visit the website but rarely make purchases.

### Cluster 1 – High Value Customers

Customers with the highest income and highest spending levels. These represent the most valuable customer segment.

### Cluster 2 – Regular Customers

Customers with moderate income and consistent purchasing behavior. They contribute steadily to overall revenue.

### Cluster 3 – Low Spending Singles

Customers who typically live alone and exhibit lower spending behavior with moderate website activity.

---

## 📊 Key Insights

* Customers with **higher income tend to spend significantly more**.
* Some users frequently browse the website but **rarely make purchases**.
* Household composition (living alone vs with a partner) influences purchasing behavior.
* Website visits do not always translate into purchases.

---

## 💼 Business Impact

Customer segmentation can help SmartCart:

* Identify **high-value customers**
* Design **personalized marketing campaigns**
* Improve **customer retention**
* Increase **conversion rates**
* Optimize **marketing budgets**

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Kneed

---

## 📁 Project Structure

```
smartcart-customer-segmentation
│
├── smartcart_clustering.ipynb
├── smartcart_customers.csv
├── requirements.txt
└── README.md
```

---

## ▶️ How to Run

Clone the repository:

```
git clone https://github.com/lakshaybamel/smartcart-customer-segmentation.git
cd smartcart-customer-segmentation
```

Install dependencies:

```
pip install -r requirements.txt
```

Run the notebook:

```
jupyter notebook smartcart_clustering.ipynb
```

---

## 🏁 Conclusion

This project demonstrates how **unsupervised machine learning techniques** can uncover hidden patterns in customer data.

By segmenting customers into meaningful groups, businesses can move from **generic marketing strategies to data-driven customer engagement**, improving both customer satisfaction and revenue.

---

## 👨‍💻 Author

**Lakshay Bamel**
