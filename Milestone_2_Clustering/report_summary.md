report = """# Milestone 2 – Clustering and Pattern Detection

**Objective:**  
To identify behavioral patterns among customers based on `customer_age` and `tenure` using clustering algorithms.

---

**Dataset Source:**  
Milestone 1 dataset: `customer_details.csv`  
Path: `/content/drive/MyDrive/Infosys _Study Track AI based Student Study Habit Recommender/Milestone1/customer_details.csv`

---

**Steps Followed:**

1. Imported the dataset from Google Drive.
2. Selected relevant features: `customer_age`, `tenure`.
3. Standardized the data using **StandardScaler**.
4. Applied **PCA (Principal Component Analysis)** for 2D visualization.
5. Used **K-Means Clustering** to form 3 distinct customer groups.
6. Visualized clusters using scatter plots and bar charts.
7. Generated summary statistics and insights for each cluster.

---

**Tools Used:**

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (StandardScaler, PCA, KMeans, Silhouette)

---

**Key Visualizations:**

- `visualizations/cluster_scatter.png` → PCA Scatter of Clusters
- `visualizations/cluster_profile_bar.png` → Cluster Profile Comparison
- `visualizations/correlation_heatmap.png` → Feature Correlation Heatmap

---

**Insights:**
| Cluster | Description | Key Traits |
|----------|--------------|------------|
| 0 | Senior, loyal customers | Older age, high tenure |
| 1 | Mid-level segment | Moderate age and tenure |
| 2 | New or young customers | Younger with low tenure |

**Observation:**  
This clustering reveals distinct patterns in customer engagement based on age and tenure, helping in understanding retention and segmentation strategies.

---

**Conclusion:**  
The clustering analysis successfully categorized customers into meaningful groups, demonstrating data-driven pattern detection for behavioral insights.

"""
with open("report_summary.md", "w") as f:
f.write(report)
