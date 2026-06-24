# Crime Pattern Analysis using PCA and Clustering

## Project Overview

This project applies Principal Component Analysis (PCA) and unsupervised machine learning techniques to the USArrests dataset. The objective is to explore relationships between violent crime rates and urban population levels across U.S. states, reduce the dimensionality of the data, and identify groups of states with similar crime characteristics.

The project demonstrates the use of:

- Exploratory Data Analysis (EDA)
- Correlation Analysis
- Principal Component Analysis (PCA)
- Hierarchical Clustering
- K-Means Clustering
- Cluster Evaluation

---

## Dataset

The dataset contains crime statistics for 50 U.S. states in 1973.

### Features

| Feature | Description |
|----------|-------------|
| Murder | Arrests for murder per 100,000 residents |
| Assault | Arrests for assault per 100,000 residents |
| UrbanPop | Percentage of the population living in urban areas |
| Rape | Arrests for rape per 100,000 residents |

### Data Source

USArrests Dataset

https://vincentarelbundock.github.io/Rdatasets/doc/datasets/USArrests.html

---

## Objectives

The main objectives of this project are:

1. Explore and understand the structure of the dataset.
2. Perform correlation analysis to identify relationships between variables.
3. Apply PCA to reduce dimensionality while retaining most of the information.
4. Visualise the first two principal components using a biplot.
5. Determine an appropriate number of principal components for further analysis.
6. Apply multiple clustering techniques.
7. Compare clustering results and evaluate cluster quality.
8. Interpret the characteristics of each cluster.

---

## Methodology

### 1. Data Exploration and Preprocessing

- Loaded and inspected the dataset.
- Checked for missing values.
- Examined summary statistics.
- Standardised variables before PCA.

### 2. Correlation Analysis

A correlation matrix and heatmap were generated to investigate relationships between crime variables and urban population percentages.

### 3. Principal Component Analysis (PCA)

PCA was applied to:

- Reduce dimensionality.
- Identify the variables contributing most to variation in the dataset.
- Visualise state relationships in lower-dimensional space.

### 4. Clustering

Two clustering techniques were applied:

#### Hierarchical Clustering

- Ward linkage method
- Dendrogram visualisation
- Cluster assignment based on dendrogram structure

#### K-Means Clustering

- Cluster assignment using principal component scores
- Comparison with hierarchical clustering results

### 5. Cluster Evaluation

Silhouette scores were used to evaluate cluster quality and compare clustering approaches.

---

## Key Findings

- Assault, Murder, and Rape exhibit strong positive correlations.
- The first two principal components capture the majority of the dataset's variance.
- PCA effectively reduces dimensionality while preserving important information.
- Clustering reveals distinct groups of states with similar crime profiles.
- K-Means clustering achieved the strongest separation between clusters based on silhouette score.

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- SciPy

---

## Repository Structure

```text
├── README.md
├── UsArrests.csv
└── crime_pattern_analysis_pca_clustering.ipynb
```

---

## Example Visualisations

The notebook includes:

- Correlation Heatmap
- PCA Explained Variance Plot
- PCA Biplot
- Hierarchical Clustering Dendrogram
- Cluster Visualisations
- Silhouette Score Comparisons

---

## Results

Principal Component Analysis successfully reduced the dimensionality of the dataset while retaining most of the information. Clustering techniques identified meaningful groups of states based on crime characteristics, demonstrating how unsupervised machine learning can uncover hidden patterns in multivariate data.

---

## Author

**Stephanie Bergh**

Junior Data Analyst | Python | Machine Learning | Data Visualisation

GitHub: https://github.com/StephanieBergh

LinkedIn: https://www.linkedin.com/in/stephanie-bergh-142aa818a/

---

## License

This project is intended for educational and portfolio purposes.
