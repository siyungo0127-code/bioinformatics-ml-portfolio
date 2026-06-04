# Cancer Transcriptomics and Machine Learning Portfolio

This repository contains bioinformatics and machine learning projects completed during my MSc studies. The projects focus on transcriptomic data analysis, molecular subtype discovery, machine learning-based classification, and biological interpretation of gene expression patterns.

The goal of this portfolio is to demonstrate practical experience in bioinformatics workflows, statistical analysis, machine learning, and cancer transcriptomics.

---

# Project Overview

## Gene Expression-Based Cancer Subtype Classification and Transcriptomic Profiling

This project combines supervised and unsupervised learning approaches to analyze cancer gene expression datasets.

### Part 1: DLBCL Cell-of-Origin Classification

A Random Forest classifier was developed to predict Diffuse Large B-Cell Lymphoma (DLBCL) Cell-of-Origin (COO) subtypes using gene expression profiles.

Main tasks:

* Training/testing cohort split
* Random Forest model development
* Hyperparameter tuning
* Feature selection
* ROC curve analysis
* Independent cohort validation

### Part 2: ESCC Molecular Subtyping

Unsupervised learning methods were used to identify molecular subtypes in Esophageal Squamous Cell Carcinoma (ESCC).

Main tasks:

* Non-negative Matrix Factorization (NMF)
* Consensus Clustering
* Differential Expression Analysis (limma)
* Signature gene identification
* Gene Set Enrichment Analysis (GSEA)
* Biological interpretation of subtype-specific pathways

---

# Skills Demonstrated

## Bioinformatics

* Gene Expression Analysis
* Differential Expression Analysis
* Cancer Transcriptomics
* Functional Enrichment Analysis
* Biological Pathway Interpretation

## Machine Learning

* Random Forest Classification
* Feature Selection
* Hyperparameter Optimization
* Model Validation
* ROC/AUC Evaluation

## Statistical Analysis

* Hypothesis Testing
* Clustering Analysis
* Biomarker Discovery

## Programming

* R
* Bioconductor
* Data Visualization
* Reproducible Research

---

# Tools and Packages

* randomForest
* caret
* pROC
* limma
* NMF
* clusterProfiler
* Biobase
* org.Hs.eg.db

---

# Repository Structure

```text
README.md

01_project_summary.md

ML-AI-LAQ1-2-assignment_SiyunPark.Rmd

ML-AI-LAQ12_SiyunPark.html

ML-AI-LAQ3_SiyunPark.ipynb

ML-AI-LAQ3_SiyunPark.html
```

---

# Key Learning Outcomes

Through these projects, I gained experience in:

* Building predictive models from high-dimensional gene expression datasets
* Identifying biologically meaningful molecular subtypes
* Performing differential expression analysis and pathway enrichment analysis
* Evaluating machine learning models using independent validation datasets
* Interpreting computational results in a biological context

---

# Future Improvements

* Refactor analyses into modular and reusable scripts
* Build reproducible bioinformatics workflows
* Containerize analyses using Docker
* Implement workflow management systems such as Nextflow
* Extend analyses to NGS-based datasets
