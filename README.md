# 🛍️ Mall Customer Segmentation using K-Means Clustering

This project implements **Customer Segmentation** using the K-Means Clustering algorithm on the Mall Customers dataset.  
The application is built with **Streamlit** for interactive visualization and prediction.

---

## 📌 Project Overview

Customer segmentation is a marketing strategy that divides customers into groups based on common characteristics.

In this project:
- We used **K-Means Clustering**
- Features used:
  - Age
  - Annual Income (k$)
  - Spending Score (1–100)
- Built an interactive **Streamlit Web App**
- Visualized clusters using 3D scatter plots and pie charts

---

## 📊 Dataset

Dataset: `Mall_Customers.csv`

Columns used:
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

Gender column was removed from clustering to match model training consistency.

---

## ⚙️ Technologies Used

- Python 3.13
- scikit-learn
- pandas
- numpy
- joblib
- plotly
- streamlit

---

## 🧠 Machine Learning Model

Algorithm Used:
- **KMeans (sklearn.cluster.KMeans)**

Steps performed:

1. Data Preprocessing
   - Selected 3 numerical features
   - Scaled data using StandardScaler

2. Model Training
   - Applied KMeans clustering
   - Defined optimal number of clusters
   - Saved trained model using joblib

3. Model Saving
   - `kmeans_model.pkl`
   - Clustered dataset saved as `clusterd_data.csv`

---

## 🚀 Streamlit Application Features

- User input via sliders:
  - Age
  - Annual Income
  - Spending Score
- Cluster prediction
- Cluster description & insights
- 3D interactive cluster visualization
- Pie chart of customer distribution
- Business recommendations for each cluster

---

## 🛠 Installation Guide

### 1️⃣ Install Python
Download from:
https://www.python.org/downloads/

Make sure to check:
- ✔ Add Python to PATH
- ✔ Install pip

---

### 2️⃣ Install Required Libraries

- pip install streamlit pandas numpy scikit-learn plotly joblib



### 3️⃣ Run the Application

Navigate to project folder:
Run:
- streamlit run Streamlit_app.py


📂 Project Structure
├── Streamlit_app.py
├── kmeans_model.pkl
├── Mall_Customers.csv
├── clusterd_data.csv
├── cluster.ipynb
├── random_forest_model.pkl
├── README.md
