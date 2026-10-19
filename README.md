# 👥 Customer Segmentation Project

An end-to-end data science and machine learning project that segments retail customers based on behavioral patterns and purchasing history using RFM Analysis and K-Means Clustering.

---

## 📌 Project Overview

Understanding customer behavior is essential for targeted marketing, customer retention, and maximizing revenue. This project leverages unsupervised machine learning to group retail customers into distinct behavioral segments (Champions, Loyal Customers, Recent Buyers, and At-Risk Users), allowing businesses to tailor their strategies effectively.

---

## 🎯 Key Features & Workflow

* **RFM Feature Engineering:** Automatically extracts and calculates **Recency** (days since last order), **Frequency** (total orders), **Monetary value** (total spend), and **Total Quantity** from transaction logs.
* **Feature Scaling:** Standardizes features using scikit-learn's `StandardScaler` to ensure balanced cluster formation.
* **K-Means Machine Learning:** Implements an unsupervised K-Means Clustering algorithm ($K=4$) to cluster customers based on similarity.


* **Data Visualization:** Generates and plots scatter charts (`customer_segmentation_plot.png`) illustrating **Order Frequency vs. Monetary Value** across all segments.


* **Model Persistence:** Exports the trained machine learning model (`kmeans_model.pkl`) and feature scaler (`scaler.pkl`) using `joblib` for future deployment or web applications.

---

## 🛠️ Tools & Technologies Used

* **Programming Language:** Python
* **Environment:** Google Colab / Jupyter Notebooks
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Joblib

---

## 📊 Customer Segment Distribution

Based on the model output, the customer base is categorized into the following groups:

* **At-Risk / Inactive:** 70 customers
* **Champions (High Value, High Freq):** 65 customers
* **Recent / Low Engagement:** 34 customers
* **Loyal Customers:** 28 customers

---

## 🚀 How to Run the Project

1. Ensure the dataset (`sales_analysis_dataset.csv`) is present in your working directory.
2. Open and run the Google Colab notebook (`Customer_Segmentation.ipynb`) or execute the Python script.
3. The script will output the cluster summary statistics, save the visualization plot, and generate the `.pkl` model files.

---
