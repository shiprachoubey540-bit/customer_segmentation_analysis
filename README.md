**Project Overview**

This project focuses on customer segmentation using clustering techniques to analyze purchasing behavior. The goal is to group customers into distinct segments based on their income, spending patterns, and purchasing frequency, helping businesses make data-driven decisions.

**Objectives**

Perform data cleaning and exploratory data analysis (EDA)
Analyze customer purchasing behavior
Identify patterns using statistical measures
Apply K-Means clustering to segment customers
Visualize different customer groups

**Dataset**


The dataset used is iFood customer data, which includes:

Demographics (Income, Recency)
Purchase behavior (Web, Catalog, Store)
Spending on different product categories
🛠️ Technologies Used
Python 
Pandas (Data manipulation)
NumPy (Numerical operations)
Matplotlib & Seaborn (Visualization)
Scikit-learn (Machine Learning)
🔍 Project Workflow
1. Data Loading
Imported dataset using Pandas
Previewed initial data
2. Data Cleaning
Checked for missing values
Removed unnecessary columns (Z_CostContact, Z_Revenue)
Handled outliers using IQR method
3. Feature Engineering
Created a new feature:
TotalPurchases = Web + Catalog + Store purchases
4. Exploratory Data Analysis (EDA)
Statistical summary of data
Average metrics:
Income
Total spending
Purchase frequency
Recency
Correlation analysis:
Income vs Spending
Web visits vs Purchases
5. Data Preprocessing
Selected important features:
Income
Recency
TotalPurchases
MntTotal
Applied Standard Scaling
6. Clustering (K-Means)
Used Elbow Method to determine optimal clusters
Applied K-Means clustering (k=4)
Assigned cluster labels to customers
7. Visualization
Scatter plot of customer segments
Bar charts for:
Average spending per cluster
Purchase frequency per cluster
Customer distribution
Recency analysis
 Key Insights
Customers can be grouped into distinct segments based on behavior
Higher income generally correlates with higher spending
Some clusters show:
High spending but low frequency
Frequent buyers with moderate spending
Helps identify high-value customers and potential targets
 Results
Customers divided into 4 clusters
Each cluster represents a unique purchasing pattern
Useful for:
Targeted marketing
Personalized recommendations
Business strategy optimization
   How to Run the Project
Install required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn
Place dataset (ifood_df.csv) in the working directory
Run the Jupyter Notebook:
jupyter notebook
📌 Future Improvements
Use advanced clustering (DBSCAN, Hierarchical)
Add more behavioral features
Deploy as a web dashboard
Integrate real-time customer data
