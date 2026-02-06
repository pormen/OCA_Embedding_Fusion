# Supplementary Data Preparation Notebook (Zenodo)

## Title
Supplementary Data Processing and Sample Weighting for Oral Cancer Image Classification

---

## Description

This repository contains a **supplementary Jupyter notebook** used to document and reproduce key data preparation steps associated with an oral cancer image classification study using deep learning and hybrid machine learning approaches.

The notebook is intended to accompany a **Zenodo data deposit** and serves as a transparent, executable record of how raw data were inspected and how **sample weighting strategies** were defined prior to model training and evaluation.

Importantly, this notebook does **not** perform model training. Its purpose is methodological transparency and reproducibility.

---

## Notebook Overview

### `Nature 1 Zenodo Note.ipynb`

The notebook is organized into two main sections:

#### 1. RAW DATA
This section focuses on:
- Loading and inspecting the raw dataset
- Verifying label structure and class distributions
- Identifying class imbalance
- Generating descriptive summaries to contextualize downstream modeling

These steps ensure that dataset composition is clearly documented before any learning-based processing is applied.

#### 2. SAMPLE WEIGHT
This section documents:
- The rationale for sample-level weighting
- Definition of instance weights based on class frequencies
- Implementation of weighting logic
- Preparation of weights for use in downstream training pipelines

Sample weighting is used to mitigate class imbalance and improve sensitivity to minority classes during model training.

---

## Intended Use

This notebook is designed to support:

- **Reproducibility**: enabling reviewers and readers to verify data handling decisions  
- **Transparency**: making preprocessing and weighting choices explicit  
- **Reuse**: allowing other researchers to adapt the weighting strategy to similar datasets  

It complements, but does not replace, the main experimental notebooks used for model training and evaluation.

---

## How to Run

1. Open the notebook using Jupyter Notebook or JupyterLab  
2. Ensure the dataset files are available in the expected directory paths  
3. Execute cells sequentially from top to bottom  

No GPU is required. The notebook is lightweight and CPU-only.

---

## Requirements

- Python 3.8+
- Jupyter Notebook
- pandas
- numpy

Optional (for visualization):
- matplotlib

---

## Relation to Main Experiments

- This notebook supports the **data preparation and sample weighting steps** used in the main classification experiments  
- Model training, evaluation, and statistical testing are conducted in separate notebooks  
- Sample weights defined here are consumed by downstream pipelines  

---

## Reproducibility Notes

- All operations are deterministic given identical input data  
- No random seeds are required  
- No stochastic optimization or training is performed  


---

## License

This notebook is released under the **MIT License**, unless otherwise specified in the associated Zenodo record.

---

## Notes for Reviewers

This notebook is provided to:
- Support methodological inspection
- Enable verification of dataset handling decisions
- Improve transparency in line with open science and data-sharing best practices
