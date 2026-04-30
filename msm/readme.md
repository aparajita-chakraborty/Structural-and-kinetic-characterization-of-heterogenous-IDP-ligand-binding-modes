# MSM/PCCA-Based Kinetic Modeling and Cluster Interaction Analysis

This folder contains the workflow for constructing **Markov State Models (MSMs)** and performing **PCCA-based macrostate analysis** for both ligands, followed by **cluster-wise intermolecular interaction characterization**.

---

## 📁 Contents

### 1. MSM Construction and PCCA Analysis
- `MSM_PCCA_combined_features_both_ligands.ipynb`

This notebook:
- Performs time-lagged dimensionality reduction (e.g., TICA)
- Constructs Markov State Models (MSMs) for both **Fasudil** and **Ligand-47**
- Validates models using:
  - Implied timescales  
  - Chapman–Kolmogorov tests  
- Applies **PCCA (Perron Cluster Cluster Analysis)** to identify metastable macrostates  
- Generates discrete trajectories (`dtraj`) defining macrostate assignments for each frame  

---

### 2. Macrostate-wise Intermolecular Interaction Analysis

- `msm_pcca_cluster_analysis_fasudil.ipynb`  
- `msm_pcca_cluster_analysis_ligand_47.ipynb`

These notebooks:
- Use the **macrostate assignments (`dtraj`)** generated from the MSM/PCCA notebook  
- Extract frames corresponding to each metastable state  
- Compute intermolecular interaction features, including:
  - Residue-level contacts  
  - Interaction frequencies  
- Visualize interaction patterns for each macrostate  
- Save macrostate-wise interaction features as `.npy` files  

---

## 🧠 Workflow Summary

1. Perform kinetic dimensionality reduction and MSM construction  
2. Validate MSM using implied timescales and CK tests  
3. Identify metastable states using PCCA  
4. Generate macrostate assignments (`dtraj`)  
5. Compute macrostate-wise intermolecular interactions for each ligand  
6. Analyze interaction patterns across metastable states  

---

## 🔁 Workflow Diagram

TICA → MSM → PCCA → Metastable States (dtraj)
↓
Macrostate Interaction Analysis (per ligand)


---

## 🎯 Purpose

This workflow links:
- **Kinetic modeling (MSM/PCCA)**  
with  
- **Biochemical interpretation (intermolecular interactions)**  

enabling identification and characterization of **metastable binding states** and their associated interaction patterns.
