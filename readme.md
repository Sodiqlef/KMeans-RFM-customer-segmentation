---
# 🧠 Customer Segmentation with K-Means (RFM Analysis)

This project applies unsupervised learning to segment customers based on their purchasing behavior using the **RFM (Recency, Frequency, Monetary)** model and **K-Means Clustering**. The goal is to help businesses identify high-value customers, re-engage low-value ones, and personalize marketing strategies.
---

## 🔍 Project Objective

Segment customers to:

- Discover **loyal, high-value buyers**
- Detect **low-value or at-risk customers**
- Support **targeted marketing strategies** and **retention efforts**

---

## 📦 Dataset

- **Source**: Kaggle
- **Description**: Includes customer transaction data for a UK-based online retail store between 2010 and 2011.

---

## 🧰 Tools & Libraries

- **Python**
- **Pandas** – data manipulation
- **Seaborn/Matplotlib** – data visualization
- **Scikit-learn** – preprocessing, scaling, K-Means, evaluation
- **NumPy**

---

## 🔗 RFM Model Explained

RFM is a customer segmentation technique based on:

| Metric    | Meaning                             |
| --------- | ----------------------------------- |
| Recency   | How recently the customer purchased |
| Frequency | How often they purchase             |
| Monetary  | How much money they spent           |

---

## 🧪 Steps Performed

1. **Exploratory Data Analysis**

   - Checked for missing values and anomalies
   - Visualized purchase distribution

2. **RFM Feature Creation**

   - Calculated Recency, Frequency, and Monetary values per customer

3. **Outlier Removal**

   - Removed top 15% of extreme values to improve clustering performance

4. **Feature Scaling**

   - Applied `StandardScaler` to normalize RFM features

5. **K-Means Clustering**

   - Evaluated cluster count using:
     - **Elbow method** (inertia)
     - **Silhouette score**

6. **Cluster Profiling**

   - Grouped customers into **two segments**:
     - Cluster 1: High-value, loyal, frequent buyers
     - Cluster 0: Low-value, infrequent or inactive customers

7. **Visualization**
   - Compared RFM values across clusters
   - Visualized cluster sizes and distributions

---

## 📈 Key Results

- **Optimal Clusters**: 2 (based on silhouette and elbow methods)
- **Insights**:
  - A small portion of customers bring the most value
  - Majority of customers are at risk or low-engagement

---

## 📊 Sample Output

```python
rfm.groupby('Cluster').mean()
```

| Cluster | Recency | Frequency | Monetary |
| ------- | ------- | --------- | -------- |
| 0       | High    | Low       | Low      |
| 1       | Low     | High      | High     |

---

## 📬 Contact

📧 Email: ogundimusodiq0@gmail.com  
🐙 GitHub: [@your-username](https://github.com/sodiqlef)

---
