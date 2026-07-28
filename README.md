<h1 align="center">🛍️ Customer Segmentation using K-Means Clustering and PCA</h1>

Name: Deepti Gupta

Reg No.: 23MEI10007

Application no.: IN26011816

Email: deepti.23mei10007@vitbhopal.ac.in

---

## 🎯 Objective

This repository contains a professional, production-quality implementation of **K-Means Clustering** to segment mall customers based on their purchasing behavior and annual income. **Principal Component Analysis (PCA)** is utilized to reduce the high-dimensional dataset into two principal components, enabling effective visualization of the formed clusters.

---

## 📊 Dataset

- **Dataset Name:** Mall Customer Segmentation Dataset
- **Kaggle Link:** [Customer Segmentation Tutorial in Python](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Rows:** 200
- **Columns:** 5

| Feature | Description |
| :--- | :--- |
| **CustomerID** | Unique ID assigned to the customer |
| **Gender** | Gender of the customer |
| **Age** | Age of the customer |
| **Annual Income (k$)** | Annual Income of the customer in thousands of dollars |
| **Spending Score (1-100)** | Score assigned by the mall based on customer behavior and spending nature |

---

## 🛠️ Technologies Used

- `Python`
- `Pandas`
- `NumPy`
- `Matplotlib`
- `Seaborn`
- `Scikit-Learn`
- `Jupyter Notebook`

---

## ⚙️ Machine Learning Workflow

1. **Data Collection:** Automatically fetching data.
2. **Data Understanding:** EDA, pairplots, and distribution analysis.
3. **Data Cleaning:** Handling missing values, dropping irrelevant columns (CustomerID).
4. **Feature Scaling:** Using `StandardScaler` to normalize dimensions.
5. **Elbow Method:** Determining the optimal number of clusters (K).
6. **K-Means Clustering:** Training the unsupervised model.
7. **Cluster Assignment:** Grouping customers.
8. **PCA:** Reducing dimensionality to 2 components.
9. **Visualization:** Plotting clusters in 2D space.
10. **Cluster Evaluation:** Silhouette, Calinski-Harabasz, and Davies-Bouldin scores.
11. **Business Insights:** Profiling clusters for marketing.
12. **Conclusion:** Summarizing findings.

---

## 📈 Results

| Metric | Score |
| :--- | :--- |
| **Optimal K** | 5 |
| **Silhouette Score** | 0.2719 |
| **Calinski-Harabasz Score** | 62.1263 |
| **Davies-Bouldin Index** | 1.1811 |

---

## 🖼️ Visual Results

### Elbow Curve
![Elbow Curve](elbow_curve.png)

### Correlation Heatmap
![Correlation Heatmap](correlation_heatmap.png)

### Customer Clusters (Income vs Spending)
![Customer Clusters](customer_clusters.png)

### PCA Cluster Visualization (2D Space)
![PCA Clusters](pca_clusters.png)

### PCA Explained Variance
![Explained Variance](explained_variance.png)

---

## 👥 Customer Segments

| Cluster Name | Customer Count | Average Income | Average Spending Score | Business Strategy |
| :--- | :--- | :--- | :--- | :--- |
| Cluster 0.0 | 51 | $46.1k | 39.3 | Target with regular promotions, seasonal sales, and bundled discounts. |\n| Cluster 1.0 | 20 | $85.2k | 14.0 | Target with regular promotions, seasonal sales, and bundled discounts. |\n| Cluster 2.0 | 42 | $60.9k | 70.2 | Target with regular promotions, seasonal sales, and bundled discounts. |\n| Cluster 3.0 | 49 | $82.1k | 54.4 | Target with regular promotions, seasonal sales, and bundled discounts. |\n| Cluster 4.0 | 38 | $38.8k | 56.2 | Target with regular promotions, seasonal sales, and bundled discounts. |\n

---

## 💡 Key Observations

1. **Optimal Number of Clusters:** The Elbow method indicated that 5 clusters optimally segment the customers without overfitting.
2. **Customer Behavior Patterns:** We clearly identified 5 distinct groups, primarily separated by their Annual Income and Spending Score. 
3. **PCA Visualization Benefits:** PCA successfully reduced 4 dimensions into 2 components while capturing enough variance to make the multi-dimensional clustering interpretable on a 2D plane.
4. **Target Marketing:** The "Premium Customers" (High Income, High Spending) segment is the most valuable and should be prioritized for loyalty programs.
5. **Untapped Potential:** The "Frugal Customers" (High Income, Low Spending) segment represents an untapped opportunity for targeted, value-oriented marketing.

---

## 📝 Conclusion

This project successfully applied **K-Means Clustering** to segment mall customers into 5 distinct behavioral groups, optimizing the segmentation using the Elbow Method and validating it through metrics like the Silhouette Score. **Principal Component Analysis (PCA)** was instrumental in projecting the multidimensional dataset into a 2D space, demonstrating a clear advantage in making complex cluster boundaries visually interpretable.

While K-Means is powerful, one limitation observed here is its sensitivity to feature scaling and spherical clusters, which required standardizing the inputs. The major advantage of PCA was dimensionality reduction without significant loss of structure. Business-wise, these insights allow mall management to pivot from mass marketing to highly targeted strategies, such as aggressive loyalty campaigns for high-spenders and value-oriented promotions for high-income/low-spending groups.

---

## 📁 Repository Structure

```text
Customer-Segmentation-KMeans-PCA/
│
├── Assignment-7.ipynb          # Fully executed Jupyter Notebook
├── README.md                   # Project documentation
├── requirements.txt            # Python dependencies
├── .gitignore                  # Git ignore file
├── elbow_curve.png             # Visualization of the Elbow Method
├── customer_clusters.png       # Scatter plot of customer clusters
├── pca_clusters.png            # Visualization of clusters after PCA
├── correlation_heatmap.png     # Feature correlation heatmap
├── explained_variance.png      # PCA explained variance bar chart
├── cluster_profiles.csv        # Aggregated data for each cluster
└── clustered_customers.csv     # Complete dataset with assigned cluster labels
```

---

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Soubhik-07-ops/Customer-Segmentation-using-K-Means-Clustering-and-PCA
   cd Customer-Segmentation-KMeans-PCA
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook:**
   ```bash
   jupyter notebook Assignment-7.ipynb
   ```

---

## ⚠️ Note

**The dataset (`Mall_Customers.csv`) is excluded from this repository due to Kaggle licensing restrictions.** Users must download it separately from the provided Kaggle link or rely on the notebook's automated download script from a public mirror.
