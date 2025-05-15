Contents:
1. Feature Extraction
Folder: Feature_extraction/
Contains notebooks for extracting features from MD simulation trajectories and saving them as .npy files for use in the Dimensionality Reduction & Clustering notebooks.

2. Dimensionality Reduction & Clustering
PCA_combined_features_both.ipynb
Performs Principal Component Analysis (PCA) for dimensionality reduction, followed by K-means clustering on the extracted features.

PCCA_combined_features_both.ipynb
Uses Time-lagged Independent Component Analysis (TICA) for dimensionality reduction, followed by K-means clustering and PCCA (Perron Cluster Cluster Analysis) to identify metastable states.

3. Intermolecular Interaction Analysis
Folder: intermolecular_analysis_of_clusters/
Contains notebooks for computing intermolecular interactions within each identified cluster. The interaction features are saved as .npy files and visualized within the corresponding clustering notebooks.

Usage:
Start with the notebooks in the Feature_extraction folder to generate feature data from MD trajectories. Then proceed with one of the dimensionality reduction notebooks to generate clusters. Finally, use the analysis notebooks in the intermolecular_analysis_of_clusters directory to explore cluster-specific interactions.
