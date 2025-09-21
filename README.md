# Mall-Customer-segmentation
🛍️ Mall Customer Segmentation using K-Means Clustering

📌 Project Overview

This project applies K-Means clustering to segment mall customers into meaningful groups based on their annual income and spending score. The goal is to identify distinct customer segments that can help businesses design effective marketing strategies, loyalty programs, and product targeting.  

📂 Dataset
Source: Mall Customer Segmentation Data (Kaggle).     

⚙️ Steps Performed

1. Data Exploration:
Checked data types and missing values.
Generated descriptive statistics  to understand distributions of income, age, and spending score.
2. Data Preprocessing:
Scaled features (Age, Annual Income, Spending Score) using StandardScaler to bring all values to the same range.
3. Finding Optimal Number of Clusters:
Used the Elbow Method to plot Within-Cluster Sum of Squares (WCSS) against number of clusters (k).
The elbow point appeared at k = 5, suggesting 5 optimal clusters.
 4. K-Means Clustering:
Trained K-Means with 5 clusters.
Plotted customer segments to visualize distribution of clusters across spending score and income.
5. Cluster Profiling (Summary Statistics):
Calculated average Age, Annual Income, and Spending Score for each cluster:
| Cluster | Age | Annual Income (k\$) | Spending Score | Segment Description                                         |
| ------- | --- | ------------------- | -------------- | ----------------------------------------------------------- |
| 0       | 55  | 48                  | 42             | Older, low income, low spending                             |
| 1       | 33  | 86                  | 82             | Young, high income, high spending (premium customers)       |
| 2       | 26  | 26                  | 75             | Young, low income, high spending                            |
| 3       | 27  | 54                  | 41             | Young, average income, moderate spending                    |
| 4       | 44  | 90                  | 18             | Middle-aged, high income, low spending  |


 📊 Visualizations
 
Elbow Method
The elbow at k = 5 suggests the best number of clusters.
Customer Segmentation Plot
The scatter plot shows five distinct clusters:
Cluster 1 (Orange): Premium, high-spending customers.
Cluster 2 (Green): Young spenders despite lower income.
Cluster 4 (Purple): Wealthy but low spenders.
Cluster 0 & 3 (Blue, Red): Less valuable or average customers.   

💡 Insights 

Target Cluster 1 with loyalty programs and premium services.
Encourage Cluster 4 to spend more through personalized offers.
Monitor Cluster 2 as they represent future potential customers despite low income.
Lower priority for Clusters 0 and 3, as they have limited spending capacity.     

🛠️ Tools Used

Python
Pandas, Numpy – Data handling
Matplotlib, Seaborn – Visualization
Scikit-learn – Scaling & clustering

✅ Conclusion

The K-Means model successfully segmented mall customers into 5 meaningful clusters. These insights can guide data-driven marketing strategies and improve customer relationship management by focusing on high-value and high-potential groups.
