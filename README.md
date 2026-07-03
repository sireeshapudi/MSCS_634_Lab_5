# MSCS_634_Lab_5

# MSCS 634 - Lab 5
## Clustering Techniques Using DBSCAN and Hierarchical Clustering

### Course
MSCS 634 – Advanced Big Data and Data Mining

### Lab Title
Lab 5: Clustering Techniques Using DBSCAN and Hierarchical Clustering

---

## Objective

The purpose of this lab was to explore two unsupervised machine learning algorithms, Agglomerative Hierarchical Clustering and DBSCAN, using the Wine dataset available in the Scikit-learn library. The lab focused on understanding how different clustering techniques organize similar observations, how parameter selection affects clustering behavior, and how clustering quality can be evaluated using multiple performance metrics.

---

## Dataset

The Wine dataset contains chemical analysis measurements collected from three different wine cultivars. Since clustering algorithms are distance-based, all numerical features were standardized using Z-score normalization before model development to ensure equal contribution from every feature.

---

## Work Completed

The following tasks were successfully completed during this lab:

- Loaded and explored the Wine dataset.
- Examined the dataset using `head()`, `info()`, and `describe()`.
- Standardized all numerical features using StandardScaler.
- Implemented Agglomerative Hierarchical Clustering.
- Generated scatter plots for multiple cluster configurations.
- Created and interpreted a hierarchical dendrogram.
- Applied DBSCAN clustering.
- Experimented with different epsilon values to study parameter sensitivity.
- Evaluated clustering performance using:
  - Silhouette Score
  - Homogeneity Score
  - Completeness Score
- Compared Hierarchical Clustering and DBSCAN using quantitative evaluation metrics and visualizations.

---

## Key Insights

- Hierarchical Clustering successfully separated the Wine dataset into meaningful groups and showed stronger agreement with the original class labels.
- The dendrogram clearly illustrated how observations merged into larger clusters, making hierarchical relationships easier to interpret.
- DBSCAN grouped observations according to data density rather than requiring a predefined number of clusters.
- The epsilon parameter significantly influenced the number of detected clusters and the amount of noise identified.
- Although DBSCAN achieved a reasonable Silhouette Score, its Homogeneity and Completeness Scores were lower because the density-based clusters did not closely match the actual wine classes.
- The comparison demonstrated that algorithm selection depends heavily on dataset characteristics and clustering objectives.

---

## Challenges Encountered

One challenge involved selecting suitable DBSCAN parameters. Different epsilon values produced noticeably different clustering results, requiring experimentation to identify meaningful clusters. Interpreting the dendrogram and comparing multiple clustering evaluation metrics also provided valuable practical experience with unsupervised learning techniques.

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy

---

## Conclusion

This lab strengthened my understanding of density-based and hierarchical clustering techniques. Hierarchical Clustering produced clusters that better represented the underlying structure of the Wine dataset, while DBSCAN demonstrated the importance of density estimation and parameter tuning. Comparing multiple evaluation metrics provided valuable insight into selecting appropriate clustering algorithms for different real-world datasets.