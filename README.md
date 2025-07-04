# Formative_1_-Sound_Clustering_HMMs
## Overview
This project explores unsupervised clustering techniques on unlabeled sound data using **Mel-frequency cepstral coefficients (MFCCs)**. The goal is to discover natural groupings within the data by applying **dimensionality reduction** and **clustering algorithms**, followed by a thorough evaluation of the results.

## Key Steps

1. **Data Preprocessing**
   - Loaded MFCC features
   - Visualized feature relationships using a **pairplot**
   - Identified redundancy and multicollinearity

2. **Dimensionality Reduction**
   - Applied **Principal Component Analysis (PCA)** and **t-SNE** to reduce feature space
   - Visualized reduced data in 2D/3D for better interpretability

3. **Clustering**
   - Implemented **K-Means** clustering
   - Implemented **DBSCAN** clustering
   - Visualized cluster results on reduced data

4. **Evaluation Metrics**
   - **Silhouette Score**
   - **Davies-Bouldin Index**
   - Interpretation of cluster compactness and separation

## Results Summary

- **K-Means**
  - Silhouette Score: `0.2519`
  - Davies-Bouldin Index: `1.4346`
  - Result: Formed three moderately distinct clusters, indicating **average performance**

- **DBSCAN**
  - Failed to form meaningful clusters
  - Most points collapsed into a single group due to **density and overlap issues**

## Key Insights

- **Dimensionality reduction** was crucial in revealing patterns hidden in the high-dimensional MFCC space.
- **K-Means** worked better due to its ability to form spherical clusters in the PCA-reduced space.
- **DBSCAN** struggled due to lack of density separation, which is common in noisy or overlapping feature sets.

## How to run the notebook
You can directly open it on colab OR
1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload the notebook file:  
   `File > Upload notebook`
3. Run the cells in order. If any required libraries are missing, you can install them directly in a cell using pip (e.g., `!pip install seaborn`).
4. Upload the unlabelled sound dataset to be able to load the data and run the codes.
