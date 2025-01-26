# RFM Analysis and Customer Clustering Project

This project focuses on using **RFM (Recency, Frequency, Monetary)** analysis and **K-Means Clustering** to segment customers based on their purchasing behavior. 
The goal is to derive actionable insights for improving marketing strategies and enhancing customer retention.

---

## 📌 Project Overview
This project aims to:
- Segment customers based on their purchasing behavior.
- Analyze key customer groups using **RFM Scores**.
- Use **K-Means Clustering** to identify customer clusters.
- Provide actionable insights for targeted marketing campaigns.

By analyzing RFM metrics, businesses can better understand their customer base and allocate resources effectively to improve customer retention and revenue.

---

## 🌟 Features
1. **RFM Score Calculation**:
   - Customers were scored on **Recency**, **Frequency**, and **Monetary Value**.
2. **Customer Segmentation**:
   - Segmented customers into distinct groups using **K-Means Clustering**.
3. **Cluster Insights**:
   - Analyzed characteristics of each cluster to derive business insights.
4. **Recommendations**:
   - Provided actionable strategies tailored to each customer segment.

---

## 📊 Dataset
- **Source**: [MySQL].
- **Calculated Columns**:
  
  - Recency (Days since last purchase)
  - Frequency (Number of purchases)
  - Monetary Value (Total spending)
  - RFM Customer Segments (Derived segments)

### RFM Customer Segments:
| RFM Segment            | Recency Score | Frequency Score | Monetary Score |
|-------------------------|---------------|-----------------|----------------|
| At Risk Customers       | 2.34          | 1.01            | 1.64           |
| Can't Lose              | 1.54          | 1.00            | 1.46           |
| Champions               | 3.81          | 3.06            | 3.23           |
| Lost                    | 1.00          | 1.00            | 1.00           |
| Potential Loyalists     | 3.92          | 1.19            | 1.74           |

---

## 💻 Technologies Used
- **SQL**: Extracted and cleaned data from a MySQL database.
- **Python**:
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.
- **Jupyter Notebook**: For analysis and visualization.

---

## 🔍 Methodology
1. **Data Extraction**:
   - Retrieved customer transaction data from MySQL.
2. **RFM Analysis**:
   - Calculated:
     - **Recency**: Days since the last purchase.
     - **Frequency**: Number of purchases.
     - **Monetary Value**: Total spending.
   - Scored customers on a scale to create RFM metrics.
3. **K-Means Clustering**:
   - Standardized RFM scores for clustering.
   - Used the **Elbow Method** to determine the optimal number of clusters.
   - Segmented customers into 4 clusters.
4. **Insights and Visualization**:
   - Plotted cluster distributions and analyzed group characteristics.

---

## 🔎 Insights and Results
### Cluster Summary:
| Cluster | Recency | Frequency | Monetary Value | Insight                              |
|---------|---------|-----------|----------------|--------------------------------------|
| 0       | 632.66  | 1.00      | 259.53         | Rare, low-value customers.           |
| 1       | 600.57  | 1.00      | 487.20         | Rare buyers with moderate spending.  |
| 2       | 621.41  | 2.09      | 1106.81        | Occasional buyers, high spenders.    |
| 3       | 629.25  | 1.00      | 765.06         | Rare buyers, slightly higher spend.  |

### RFM Segment Performance:
| Segment                 | Avg Recency | Avg Frequency | Avg Monetary Value |
|-------------------------|-------------|---------------|---------------------|
| At Risk Customers       | 626.62      | 1.01          | 553.82              |
| Can't Lose              | 635.55      | 1.00          | 458.83              |
| Champions               | 608.45      | 2.03          | 1279.26             |
| Lost                    | 643.00      | 1.00          | 241.56              |
| Potential Loyalists     | 607.35      | 1.10          | 588.52              |

---

## 🎯 Recommendations
### For Each Cluster:
1. **Cluster 0 (Low Engagement, Low Spending)**:
   - Strategy: Re-engage these customers with discounts or incentives.
   - Focus: Email marketing and affordability.
2. **Cluster 1 (Rare Buyers, Moderate Spend)**:
   - Strategy: Encourage frequent purchases using loyalty programs.
   - Focus: Value-added offers and bundling.
3. **Cluster 2 (High-Value, Occasional Buyers)**:
   - Strategy: Maintain engagement through exclusive deals.
   - Focus: Personalized offers and early access.
4. **Cluster 3 (Rare Buyers, Slightly Higher Spend)**:
   - Strategy: Boost purchase frequency with targeted promotions.
   - Focus: Product recommendations and discounts.

---

## RFM Insights Visuals

![image]()

![image]()

![image]()

---

## Cluster Insights Visuals

![image](https://github.com/Shaikh-areeb/RFM_Analysis_And_Customer_Segmentation-Clustering/blob/main/insights%20images/Screenshot%202025-01-26%20230633.png
)

