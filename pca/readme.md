# PCA-Based Clustering and Intermolecular Interaction Analysis

This folder contains the workflow for performing **Principal Component Analysis (PCA)** and analyzing **cluster-specific intermolecular interactions** for both ligands.

---

## 📁 Contents

### 1. PCA and Clustering
- `PCA_combined_features_both_ligands.ipynb`

This notebook:
- Performs PCA on intermolecular feature representations for both **Fasudil** and **Ligand-47**
- Clusters conformations in the reduced dimensional space
- Generates discrete trajectories (`dtraj`) defining cluster assignments for each frame

---

### 2. Cluster-wise Intermolecular Interaction Analysis

- `fasudil_cluster_interactions.ipynb`  
- `lig47_cluster_interactions.ipynb`

These notebooks:
- Use the **cluster assignments (`dtraj`)** generated from the PCA notebook
- Extract frames corresponding to each cluster for each ligand
- Compute intermolecular interaction features, including:
  - Residue-level contacts  
  - Interaction frequencies  
- Visualize interaction patterns for each cluster  
- Save cluster-wise interaction features as `.npy` files  

---

### 3. Comparative Visualization

The saved interaction feature files are:
- Reloaded into `PCA_combined_features_both_ligands.ipynb`
- Used to visualize and compare intermolecular interaction patterns across clusters for both ligands **side by side**

---

## 🧠 Workflow Summary

1. Perform PCA and clustering  
2. Generate cluster assignments (`dtraj`)  
3. Compute cluster-wise intermolecular interactions for each ligand  
4. Save interaction features  
5. Reload and compare interaction patterns across ligands  

---

## 🔁 Workflow Diagram

PCA → Clusters → dtraj
↓
Cluster Interaction Analysis (per ligand)
↓
Comparative Visualization


---

## 🎯 Purpose

This workflow links:
- **Structural clustering (PCA)**  
with  
- **Biochemical interpretation (intermolecular interactions)**  

enabling direct comparison of how different ligands interact with the protein across shared conformational states.
