# Student Stress Analysis

An academic data analysis project developed to investigate the factors contributing to student stress, using unsupervised machine learning on the `StudentStress.csv` dataset.

## Project Structure

The data modeling and exploration were divided into three main stages, documented in modular Jupyter Notebooks:

* **`notebook1.ipynb`**: Dataset loading, initial cleaning, and standardization (`StandardScaler`). Application of Principal Component Analysis (PCA) and the elbow method for dimensionality reduction.
* **`notebook2.ipynb`**: Implementation of the K-Means algorithm to cluster the students and visualization of the discovered groups.
* **`notebook3.ipynb`**: Visualization of the Hierarchical Clustering algorithm through a Dendrogram, and application of the t-SNE method to detect complex, non-linear relationships.

## Key Findings

The modeling based on unsupervised learning revealed distinct behavioral patterns among students regarding their perception of study load:

* **Dimensionality Reduction (PCA and t-SNE):** PCA reduced the dataset to two dimensions, preserving 50.13% of the total variance. The t-SNE mapping proved that the relationship between academic and health variables is complex and non-linear, forming well-defined groups.
* **Profile Identification (K-Means and Dendrogram):** The application of the elbow method and hierarchical analysis (with a cut-off line at y=24) defined the optimal division of the data into 3 distinct clusters.
* **Group Characterization:**
  * **Group 0:** Very good academic performance and low stress level. They sleep well, rarely suffer from headaches, consider their study load low, and exercise regularly.
  * **Group 1:** Good academic performance and a relatively high stress level. They experience occasional headaches, sleep well, have a relatively high study load, and practice physical activities occasionally.
  * **Group 2:** Low academic performance and low stress. They study little, engage in minimal physical exercise, have occasional headaches, and sleep well.

## Prerequisites and Installation

To ensure environment reproducibility, all dependencies are mapped in the `requirements.txt` file.

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/irisdias1/Student-Stress-Analysis.git](https://github.com/irisdias1/Student-Stress-Analysis.git)
