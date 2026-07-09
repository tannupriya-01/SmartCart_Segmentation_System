# SmartCart Customer Segmentation System

## Project Overview :

The SmartCart Customer Segmentation System is a Machine Learning project that segments customers into distinct groups based on demographic information and purchasing behavior. The project helps businesses better understand customer profiles, enabling personalized marketing strategies and improve customer engagement.

This project includes complete data preprocessing, feature engineering, exploratory data analysis, dimensionality reduction using Principal Component Analysis (PCA), and customer segmentation using clustering algorithms.

## Problem Statement :

Businesses often have customers with different purchasing habits, incomes, and lifestyles. Treating every customer the same reduces the effectiveness of marketing campaigns.
The goal of this project is to identify similar groups of customers using unsupervised machine learning techniques so that businesses can target each customer segment more effectively.

## Dataset

The dataset contains customer information such as:

- Education
- Marital Status
- Income
- Year of Birth
- Customer Registration Date
- Product Spending
- Number of Children
- Campaign Responses
- Purchase Channels
- Website Visits
- Complaints

> **Note:** The dataset (`smartcart_customers.csv`) is not included in this repository.

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed
- Jupyter Notebook

# Workflow

## 1. Data Loading

- Loaded the customer dataset using Pandas.
- Examined the dataset using `df.info()`.

## 2. Data Cleaning

- Filled missing values in the **Income** column using the median.
- Converted customer registration dates into datetime format.

## 3. Feature Engineering

Created several new features:

- **Age**
- **Customer Tenure (Days)**
- **Total Spending**
- **Total Children**
- **Living_With**

Education categories were simplified into broader groups.

## 4. Data Preprocessing

- Removed unnecessary columns.
- Performed One-Hot Encoding on categorical variables.
- Standardized all features using StandardScaler.

## 5. Exploratory Data Analysis

Performed Pair Plot and Correlation Heatmap to understand relationships among features.

## 6. Outlier Removal

Removed extreme outliers based on Age and Income to improve clustering quality.

## 7. Principal Component Analysis (PCA)

- Applied PCA to reduce the dataset into three principal components.
- Generated a 3D visualization of the transformed data.

## 8. K-Means Clustering

- Implemented K-Means clustering on the PCA-transformed dataset.
- Used Elbow Method and KneeLocator to estimate an appropriate number of clusters.

## 9. Agglomerative Clustering

- Applied Agglomerative Clustering using Ward linkage.
- Generated 3D Cluster Visualization and Cluster Distribution Plot

## 10. Cluster Analysis

Calculated the average values of each feature within every cluster to better understand customer characteristics and purchasing behavior.

# Visualizations

The project includes:

- Pair Plot
- Correlation Heatmap
- PCA 3D Projection
- Elbow Curve
- K-Means Cluster Visualization
- Agglomerative Cluster Visualization
- Cluster Count Plot

# Project Structure

SmartCart_Segmentation_System/
│
├── Smartcart_Customers.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── smartcart_customers.csv (Not Included)

# Installation

Clone the repository:

```bash
git clone <repository-url>
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kneed
```

Place your own copy of `smartcart_customers.csv` inside the project folder.

Open the notebook and run all cells.

#  Future Improvements

- Interactive dashboard using Streamlit
- Customer recommendation system
- Automatic cluster profiling
- Real-time customer segmentation
- Model deployment using Flask or FastAPI

# Author - Tannu Priya

Machine Learning | Data Analytics | Python