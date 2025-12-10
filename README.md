# Institutional Distance, Developmental Elasticity, and OECD Convergence  
**Replication Package — Vallarino & Loaiza Keel (2025)**

This repository contains all replication materials for the paper  
**"Institutional Distance, Developmental Elasticity, and OECD Convergence"**  
by Diego Vallarino and Carlos Loaiza Keel (2025).

The repo includes data, Python code, LaTeX files, and the computational workflow used to generate the institutional embedding, distance measures, counterfactual simulations, and the Expected Developmental Shift (EDS).

---

## Repository Structure

```
/latex/               → LaTeX source files and PDFs of the paper  
/scripts/             → Python scripts for embeddings and simulations  
/figures/             → All figures used in the paper  
/data_raw/            → Raw datasets (WDI, GDL, ECI, COMTRADE, etc.)  
/data_processed/      → Cleaned data used for modeling  
/replication/         → End-to-end scripts to reproduce all results  
README.md             → This file  
.gitignore            → Ignored files for version control
```

---

## Requirements

### Python packages
- numpy  
- pandas  
- scikit-learn  
- torch  
- matplotlib  
- seaborn  
- umap-learn  

All computation is performed in Python.

---

## Replication Instructions (Python Only)

### 1. Run the master replication script in Python

```
python replication/run_all.py
```

(or run it cell-by-cell inside a Jupyter notebook)

This script automatically:

1. Loads raw institutional, structural, and governance indicators.  
2. Constructs the institutional embedding using PCA or UMAP.  
3. Computes structural distances to OECD clusters.  
4. Generates counterfactual institutional states via a conditional GAN implemented in PyTorch.  
5. Predicts development outcomes under convergence scenarios.  
6. Computes the Expected Developmental Shift (EDS).  
7. Exports all figures into `/figures/`.  
8. Outputs cleaned tables into `/data_processed/`.  

---

## Main Outputs

The replication pipeline produces:

- Institutional positioning map (Figure 2)  
- Radar institutional signatures (Figure 3)  
- Distance–EDS elasticity curve (Figure 4)  
- 20-year counterfactual trajectories (Figure 5)  
- Cross-country EDS comparisons (Figure 6)

All figures in the published PDF are reproducible from the Python scripts.

---

## Conceptual Summary

The paper introduces:

- A geometric representation of institutional systems using PCA or UMAP embeddings  
- A measure of structural distance between Latin American countries and OECD clusters  
- A generative counterfactual model for institutional convergence  
- The Expected Developmental Shift (EDS):  
  the predicted long-run development gain from institutional realignment toward OECD architectures  

This approach combines institutional economics, structural embeddings, and modern counterfactual modeling.

---

## Citation

```
Vallarino, D., & Loaiza Keel, C. (2025). Institutional Distance, Developmental Elasticity, and OECD Convergence. Working Paper
```

---

## Contact

**Diego Vallarino**  
Inter-American Development Bank  
Washington, DC  
Email: diego.vallarino@idb.org  
Website: https://diegovallarino.com

---

© 2025 — All rights reserved.
