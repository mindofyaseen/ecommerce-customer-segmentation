# 🛒 Customer Segmentation using RFM & Clustering

## 📌 Project Overview
This project applies **Clustering Analysis (KMeans)** on an Online Retail Transactions dataset.  

The goal is to:
- Clean and preprocess the raw dataset.
- Generate **Recency, Frequency, and Monetary (RFM)** metrics for customers.
- Apply **KMeans clustering** to segment customers into groups.
- Validate clusters using **Silhouette Score**.
- Create **customer personas** for better business understanding.
- Visualize results using plots and charts.

---

## 📂 Dataset
- File: `Retail_Transactions_Dataset.csv`  
- Contains customer transaction details:
  - `Transaction_ID`
  - `Customer_Name`
  - `Date`
  - `Total_Cost`
  - `Total_Items`
  - `Promotion` (categorical)

---

## ⚙️ Steps in the Notebook

### 1️⃣ Data Cleaning
- Convert `Date` to datetime format.
- Handle missing values:
  - Numeric → filled with **median**.
  - Categorical → filled with **mode**.
- Remove duplicates.
- Remove outliers using **IQR method**.
- Normalize important numeric features using **StandardScaler**.

### 2️⃣ Feature Engineering (RFM)
- **Recency** → Days since last purchase.  
- **Frequency** → Number of transactions.  
- **Monetary** → Total spend.  

### 3️⃣ Clustering
- Apply **KMeans** clustering with k=3–6.
- Select optimal **k** using **Elbow Method**.
- Validate with **Silhouette Score** (target > 0.5).
- Assign final clusters to each customer.

### 4️⃣ Cluster Personas
- Create summaries for each cluster:
  - Avg Recency
  - Avg Frequency
  - Avg Monetary
  - Number of customers
- Define customer personas (e.g., "High Value", "At Risk", "New Customers").

### 5️⃣ Visualization
- Elbow curve (to find best k).
- Silhouette scores.
- Cluster distribution (bar plot).
- RFM boxplots by cluster.
- Heatmap of average RFM values.
- 2D Scatter plots.
- Radar charts for cluster personas.

---

## 📊 Insights from the Analysis
- Different customer segments show distinct purchasing patterns.
- Business can use these clusters to:
  - Design targeted promotions.
  - Improve customer retention.
  - Identify high-value customers.

---

## 🚀 Tech Stack
- **Python Libraries:**  
  - pandas, numpy  
  - matplotlib, seaborn  
  - scikit-learn  

---

## 📝 How to Run

1. **Clone the repository**
2. **Install dependencies (Requirements.txt)**
3. **Place dataset in the project root**
4. **Run Jupyter Notebook**

---

## 📌 Author
- Muhammad Yaseen  
