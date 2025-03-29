# Customer Segmentation using Clustering

## 📌 Project Overview
This project applies **K-Means Clustering** to segment customers based on their purchasing behavior. The goal is to identify distinct customer groups that businesses can target with personalized marketing strategies.

## 📂 Dataset
The dataset used for this project contains the following key features:
- **Annual Income** (Customer's yearly earnings)
- **Spending Score** (Customer's spending behavior score assigned by the business)
- Additional demographic or transactional data (if available)

## 🚀 Steps Followed

### 1️⃣ Data Preprocessing
- Loaded the dataset using `pandas`.
- Checked for **missing values** and handled them appropriately.
- Selected **relevant features** (`Annual Income` & `Spending Score`) for clustering.
- Scaled the data using **StandardScaler** to normalize numerical values.

### 2️⃣ Finding Optimal Clusters (Elbow Method)
- Used the **Within-Cluster Sum of Squares (WCSS)** to determine the best number of clusters.
- Plotted the **Elbow Curve** to find the optimal `k`.

### 3️⃣ Applying K-Means Clustering
- Applied **K-Means Algorithm** with the chosen number of clusters.
- Assigned cluster labels to each customer.

### 4️⃣ Visualizing the Clusters
- Created a **scatter plot** to visualize customer segmentation.
- Used different colors to distinguish customer groups based on clustering.

### 5️⃣ Interpreting the Results
- Identified different customer groups such as:
  - **High Income, High Spending** (VIP Customers)
  - **Low Income, High Spending** (Potential Risky Customers)
  - **Moderate Income, Moderate Spending** (Average Customers)

### 6️⃣ Saving the Results
- Exported the final dataset with assigned clusters to a CSV file:
  ```python
  df.to_csv("customer_segments.csv", index=False)
  ```

## 📊 Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)
- **Machine Learning** (K-Means Clustering)

## 🛠️ How to Run the Project
1. Install required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
2. Run the Python script:
   ```bash
   python customer_segmentation.py
   ```
3. View the generated **customer_segments.csv** file for results.

## 🔥 Next Steps
- Experiment with **Hierarchical Clustering** and **DBSCAN**.
- Add more features (Age, Gender, Transaction History) to improve segmentation.
- Deploy as a web app using **Flask** or **Streamlit**.

---
🎯 **Project Complete!** 🚀 Let me know if you want to extend this further!

