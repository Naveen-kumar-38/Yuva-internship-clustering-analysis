# YUVA Internship – Week 3
## Unsupervised Learning and Clustering Analysis

This project was completed as part of the YUVA Internship – Virtual Data Science with Python Trainee program.

## Objective

The objective of this task is to apply unsupervised learning techniques to a publicly available dataset and identify meaningful groups within the data using clustering.

## Dataset

The UCI Automobile Dataset was used for this project. It contains information about automobiles including vehicle dimensions, engine specifications, horsepower, fuel efficiency, and price.

The dataset contains 205 records and 26 attributes.

## Methodology

The following steps were performed:

1. Loaded and explored the cleaned automobile dataset.
2. Selected nine numerical features for clustering.
3. Excluded price from the clustering inputs.
4. Standardized the selected features using StandardScaler.
5. Evaluated different cluster counts using the Elbow Method.
6. Calculated Silhouette Scores for K values from 2 to 10.
7. Selected K = 2 based on the highest Silhouette Score.
8. Applied K-Means clustering.
9. Used PCA to visualize the clusters in two dimensions.
10. Analyzed the characteristics of each cluster.
11. Compared cluster characteristics including price after clustering.
12. Validated and exported the clustering results.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Results

The analysis produced two automobile clusters.

- Cluster 0: 129 automobiles
- Cluster 1: 76 automobiles

Cluster 0 generally contains relatively smaller, lighter, lower-powered and more fuel-efficient automobiles.

Cluster 1 generally contains relatively larger, heavier, higher-powered and lower-fuel-efficiency automobiles.

Price was not used as a clustering feature. It was analyzed afterward to provide additional context about the resulting segments.

## Project Structure

```text
├── data
│   └── cleaned_automobile.csv
├── screenshots
│   ├── 01_dataset_overview.png
│   ├── ...
│   └── 12_final_validation.png
├── output
│   ├── clustered_automobile.csv
│   ├── cluster_summary.csv
│   └── clustering_metrics.csv
├── Task_3_Clustering.ipynb
└── README.md
