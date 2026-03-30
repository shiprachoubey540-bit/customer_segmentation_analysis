Customer Segmentation Analysis using K-Means
📌 Project Overview

This project focuses on customer segmentation using data analysis and machine learning techniques. The goal is to identify distinct groups of customers based on their income, spending behavior, and purchase patterns, helping businesses make data-driven marketing decisions.

📂 Dataset

The dataset used is iFood customer data, which includes:

Demographics (Income, Age proxy)
Purchase behavior (Web, Store, Catalog purchases)
Spending across product categories
Recency (last purchase)
Website activity
⚙️ Project Workflow
1. Data Preprocessing
Loaded dataset using Pandas
Checked for missing values and handled them
Removed unnecessary columns:
Z_CostContact
Z_Revenue
2. Exploratory Data Analysis (EDA)
Summary statistics (mean, std, etc.)
Unique value counts
Correlation analysis
Product-wise spending insights
3. Outlier Detection
Used IQR method to detect outliers in MntTotal
Visualized using boxplots
Filtered extreme values to improve model accuracy
4. Feature Engineering

Created a new feature:

TotalPurchases = Web + Catalog + Store Purchases

Key features selected for clustering:

Income
Recency
TotalPurchases
Total Spending (MntTotal)
5. Feature Scaling
Applied StandardScaler to normalize data
6. Clustering (K-Means)
Used Elbow Method to find optimal clusters
Selected K = 4 clusters
Applied K-Means clustering
📈 Results & Analysis
🔹 Key Metrics (Overall)
Average Income → Represents customer purchasing power
Average Spending (MntTotal) → Indicates overall engagement
Average Purchase Frequency → Shows buying behavior
Average Recency → Helps identify active vs inactive users
🔹 Correlation Insights
Positive correlation between Income and Spending
→ Higher income customers tend to spend more
Relationship between:
Website visits
Purchase frequency
→ Helps understand digital engagement
🔹 Customer Segments (Clusters)
🟢 Cluster 0 – High Value Customers
High income
High spending
Frequent purchases
👉 Strategy: Premium offers, loyalty programs
🔵 Cluster 1 – Regular Customers
متوسط income and spending
Moderate purchase frequency
👉 Strategy: Personalized recommendations
🟡 Cluster 2 – Low Engagement Customers
Low spending
Low purchase frequency
👉 Strategy: Discounts, re-engagement campaigns
🔴 Cluster 3 – Recent but Low Spending
Recent activity but low purchases
👉 Strategy: Upselling and cross-selling
🔹 Cluster Distribution
Balanced segmentation across 4 groups
Helps in targeted marketing strategies
📊 Business Insights
High-income customers contribute significantly to revenue
Recency plays a key role in identifying active users
Digital engagement (web visits) influences purchasing behavior
Product category analysis helps in targeted promotions
🚀 Applications
Personalized marketing
Customer retention strategies
Targeted advertising
Product recommendation systems
🛠️ Tech Stack
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn (KMeans, StandardScaler)
📌 Conclusion

This project successfully segments customers into meaningful groups using K-Means clustering, enabling businesses to:

Understand customer behavior
Improve marketing strategies
Increase revenue through targeted actions
📎 Future Improvements
Use advanced models (DBSCAN, Hierarchical Clustering)
Add more behavioral features
Deploy as a dashboard (Power BI / Streamlit)
