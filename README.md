# Structural-and-kinetic-characterization-of-heterogenous-IDP-ligand-binding-modes

This repository contains a computational workflow for analyzing ligand binding to intrinsically disordered proteins (IDPs), with a focus on **α-synuclein** and two ligands: **Fasudil** and **Ligand-47**.

The project integrates:
- Structural analysis  
- Kinetic modeling  
- Direct binding event characterization  

to provide a unified understanding of ligand-dependent binding mechanisms.

---

## 📁 Repository Structure

### 1. Feature Extraction
**`feature_extraction/`**

- Converts molecular dynamics trajectories into **intermolecular interaction features**
- Includes:
  - Contact-based features  
  - Hydrogen bonding  
  - Residue-level interaction descriptors  

---

### 2. PCA-Based Analysis
**`PCA/`**

- Performs **Principal Component Analysis (PCA)** on interaction features  
- Clusters conformations in reduced dimensional space  
- Computes **cluster-wise intermolecular interactions**  
- Enables **side-by-side comparison of ligands across structural states**

---

### 3. MSM/PCCA-Based Kinetic Modeling
**`MSM/`**

- Constructs **Markov State Models (MSMs)**  
- Applies **PCCA** to identify metastable states  
- Validates models using:
  - Implied timescales  
  - Chapman–Kolmogorov tests  
- Analyzes **macrostate-specific interaction patterns**

---

### 4. Binding Event Analysis
**`binding_events/`**

- Identifies **binding/unbinding events directly from trajectories**  
- Computes **residence times**  
- Focuses on **longest binding events**  
- Analyzes **residue-level interaction patterns during these events**  
- Enables **direct kinetic interpretation of binding stability**

---

## 🧠 Conceptual Workflow

Feature Extraction → Intermolecular Interaction Features → PCA → Structural Clusters
↓
MSM/PCCA → Metastable States
↓
Binding Events → Residence Time Analysis
↓
Interaction Interpretation & Comparison


---

## 🎯 Purpose

This project aims to:

- Characterize **ligand binding mechanisms in IDPs**
- Compare **binding behavior across different ligands**
- Identify **metastable binding states**
- Link:
  - Structural clustering (PCA)  
  - Kinetic modeling (MSM/PCCA)  
  - Direct time-resolved binding events  

---

## 🧩 Project Design

Each folder contains:
- Well-documented notebooks  
- Annotated workflows  
- A dedicated `README.md` explaining the specific analysis  

This modular structure allows:
- Independent exploration of each analysis type  
- Easy extension to additional ligands or systems  

---

## 📄 Associated Work

📌 *[link to your paper here]*

---

## 📬 Contact

For questions, collaborations, or discussion:

📧 *[email here]*

---

## 🌱 Notes

- All analyses are based on intermolecular interaction features derived from molecular dynamics simulations  
- The workflows are designed to be modular and reusable  
- Notebooks include annotations explaining methodology and interpretation  
