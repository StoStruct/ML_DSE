# Explainable Machine Learning-Assisted Multi-Objective Design Space Exploration of Steel Frame Buildings Considering Seismic Loss and Recovery Performance

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Overview

This repository accompanies the manuscript

> **Explainable Machine Learning-Assisted Multi-Objective Design Space Exploration of Steel Frame Buildings Considering Seismic Loss and Recovery Performance**

submitted to *Earthquake Engineering & Structural Dynamics (EESD)*.

The repository provides the complete Python implementation used to develop, evaluate, and interpret the explainability-assisted machine learning framework presented in the paper. It is intended to facilitate transparency, reproducibility, and future research in performance-based earthquake engineering (PBEE), structural resilience, and explainable artificial intelligence (XAI).

---

## Research Objective

Performance-based seismic design often requires thousands of nonlinear analyses to evaluate competing structural design alternatives.

This work develops an explainable machine learning framework that enables efficient multi-objective design space exploration while preserving engineering interpretability.

Unlike conventional surrogate models that primarily focus on prediction accuracy, the proposed framework combines machine learning with explainability techniques to extract transparent engineering knowledge regarding:

- seismic economic loss
- functional recovery
- structural design trade-offs
- resilient design recommendations

---

## Framework

The framework integrates

- Random Forest surrogate models
- Geometry-conditioned synthetic sampling
- SHAP feature attribution
- Accumulated Local Effects (ALE)
- Sobol sensitivity analysis
- Pareto-front exploration
- Decision-tree-based engineering rule extraction

---

## Repository Structure

```
.
├── notebooks/
│   └── Explainable_PBSD_Framework.ipynb
│
├── data/
│   └── BuildingDatabase.xlsx
│
├── figures/
├── results/
├── requirements.txt
└── README.md
```

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<username>/<repository>.git
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter

```bash
jupyter notebook
```

Open

```
notebooks/Explainable_PBSD_Framework.ipynb
```

and execute the notebook sequentially from top to bottom.

---

## Workflow

The notebook follows the same workflow presented in the manuscript:

1. Load structural database
2. Data preprocessing
3. Train surrogate models
4. Evaluate model performance
5. Generate geometry-conditioned synthetic samples
6. Perform explainability analyses
7. Explore Pareto-optimal designs
8. Extract interpretable engineering design rules

To improve computational efficiency and reproducibility, geometry-conditioned synthetic samples are generated once and reused throughout all explainability analyses.

---

## Data

The repository contains the processed structural database used for the analyses presented in the manuscript.

Each row corresponds to a steel Special Moment Resisting Frame (SMRF) design.

The repository includes all variables required to reproduce the reported machine learning models and explainability analyses.

---

## Reproducibility

Random seeds are fixed whenever applicable.

Executing the notebook reproduces the principal analyses reported in the manuscript, including

- surrogate model development
- SHAP analysis
- ALE plots
- Sobol sensitivity indices
- Pareto-front identification
- decision-tree interpretation

---

## Citation

If you use this repository in your research, please cite

> Mohsen Zaker Esteghamati.
>
> *Explainable Machine Learning-Assisted Multi-Objective Design Space Exploration of Steel Frame Buildings Considering Seismic Loss and Recovery Performance.*
>
> Earthquake Engineering & Structural Dynamics.
>
> DOI: (to be added after publication)

---

## License

This repository is distributed under the MIT License.

---

## Contact

**Mohsen Zaker Esteghamati, Ph.D.**

Assistant Professor

Department of Civil and Environmental Engineering

Utah State University

Email: mohsen.zaker@usu.edu

---

## Disclaimer

This software is intended for research and educational purposes.

Although the implementation has been carefully verified, no warranty is expressed or implied. Users are responsible for independently verifying results before applying them to engineering practice.
