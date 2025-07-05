AI-ML_Mall_Task8
This project uses K-Means Clustering to segment mall customers based on their annual income and spending score. It helps identify different customer types for targeted marketing. The model groups similar customers into clusters for better business insights and decision-making.

Mall Customer Segmentation using K-Means

Title:- Customer Segmentation using K-Means Clustering

Objective:

The objective of this project is to apply unsupervised machine learning using K-Means Clustering to segment mall customers into distinct groups based on their annual income and spending behavior. This helps businesses understand customer types and tailor marketing strategies accordingly.

---

Dataset:
The dataset used is: Mall\_Customers.csv

Columns in the Dataset:

| Column Name              | Description                                                                |
| ------------------------ | -------------------------------------------------------------------------- |
| `CustomerID`             | Unique identifier for each customer                                        |
| `Gender`                 | Gender of the customer (Male/Female)                                       |
| `Age`                    | Age of the customer                                                        |
| `Annual Income (k$)`     | Annual income of the customer (in thousand dollars)                        |
| `Spending Score (1-100)` | Score assigned by the mall based on customer behavior and spending pattern |


Columns Used in Clustering:

* `Annual Income (k$)`
* `Spending Score (1-100)`

These two features were selected because they directly reflect purchasing power and consumer behavior, which are most relevant for segmentation.


Tools & Libraries Used:

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn

---

 Steps Followed:

1. Import Libraries: Loaded necessary Python libraries for data analysis and visualization.
2. Load Data: Read the dataset and explored the structure using `.head()`, `.info()`, and `.describe()`.
3. Data Cleaning: Verified and confirmed that there are no missing values.
4. Feature Selection: Chose relevant columns: `Annual Income (k$)` and `Spending Score (1-100)`.
5. Data Scaling: Standardized the selected features using `StandardScaler`.
6. Determine Optimal K:

   * Used the Elbow Method to determine the optimal number of clusters.
7. K-Means Clustering:

   * Applied K-Means with the chosen number of clusters (K=5).
   * Added the cluster labels to the dataset.
    
8. Cluster Visualization:

   * Plotted clusters using `matplotlib` and `seaborn`.
9. Evaluation:

   * Calculated Silhouette Score to measure clustering performance.
10. PCA Visualization (Optional):
   * Used Principal Component Analysis to reduce dimensions and visualize clusters in 2D.

---
📊 Visual Output:

* Elbow Curve to identify optimal number of clusters.
* Scatter Plot to show clusters based on income and spending score.
* PCA Plot to visualize high-dimensional data in 2D.


Output:

Each customer is labeled with a cluster ID (0 to K-1), representing the group they belong to. These clusters can help:

* Identify high-spending vs low-spending customers
* Recognize customer segments for personalized marketing
* Optimize resource allocation based on behavior clusters


