This repository provides a framework for extracting features from molecular dynamics (MD) simulation trajectories, followed by dimensionality reduction, clustering, and cluster-based analysis of intermolecular interactions.

Contents:
1. Dimensionality Reduction & Clustering
PCA_combined_features_both.ipynb
Performs Principal Component Analysis (PCA) for dimensionality reduction, followed by K-means clustering on the extracted features.

PCCA_combined_features_both.ipynb
Uses Time-lagged Independent Component Analysis (TICA) for dimensionality reduction, followed by K-means clustering and PCCA (Perron Cluster Cluster Analysis) to identify metastable states.

2. Intermolecular Interaction Analysis
Folder: intermolecular_analysis_of_clusters/
Contains notebooks for computing intermolecular interactions within each identified cluster. The interaction features are saved as .npy files and visualized within the corresponding clustering notebooks.

Usage:

Start with one of the dimensionality reduction notebooks to generate clusters, then use the analysis notebooks in the intermolecular_analysis_of_clusters directory to explore cluster-specific interactions.
