# Binding Event and Residence Time Analysis

This folder contains the workflow for identifying **binding events directly from trajectories** and analyzing their **residence times** and **intermolecular interaction patterns** for both ligands.

---

## 📁 Contents

### 1. Residence Time Analysis (Per Residue)

- `binding_events_fasudil.ipynb`  
- `binding_events_lig_47.ipynb`

These notebooks:
- Identify binding and unbinding events from trajectory data  
- Extract continuous binding segments  
- Compute **residence times** for binding events  
- Focus on the **two longest binding events** for each ligand  
- Visualize **per-residue binding contributions** during these events  

---

### 2. Intermolecular Interaction Analysis of Binding Events

- `binding_event_analysis_fasudil.ipynb`  
- `binding_event_analysis_lig_47.ipynb`

These notebooks:
- Analyze intermolecular interactions between the ligand and protein residues  
- Focus on the **four longest binding events**  
- Compute and visualize:
  - Residue-level contacts  
  - Interaction frequencies  
- Provide detailed interaction fingerprints for long-lived binding events  

---

### 3. Comparative Visualization

- `binding_event_analysis_both_ligands.ipynb`

This notebook:
- Loads interaction data from ligand-specific analyses  
- Visualizes intermolecular interaction patterns for both ligands  
- Enables **side-by-side comparison** of binding behavior across the longest events  

---

## 🧠 Workflow Summary

1. Identify binding/unbinding events from trajectory data  
2. Extract continuous binding segments  
3. Compute residence times for each event  
4. Select longest binding events  
5. Analyze intermolecular interactions for these events  
6. Compare interaction patterns across ligands  

---

## 🔁 Workflow Diagram

Binding Detection → Binding Events → Residence Time
↓
Longest Binding Events (per ligand)
↓
Interaction Analysis (per ligand)
↓
Comparative Visualization (both ligands)


---

## 🎯 Purpose

This workflow provides a **direct kinetic perspective** on ligand binding by:

- Identifying **long-lived binding events**  
- Quantifying **residence times**  
- Characterizing **residue-level interaction patterns** during these events  

---

## ⭐ Key Insight

Long-lived binding events identified here can be directly related to:
- **Metastable states from MSM/PCCA analysis**  
- **Distinct interaction patterns observed in cluster-based analysis**  

This strengthens the interpretation of ligand-specific binding mechanisms.
