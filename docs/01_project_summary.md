# Project Summary

## Project Title

Gene Expression-Based Cancer Subtype Classification and Transcriptomic Profiling

---

## Overview

This project explores machine learning and transcriptomic analysis approaches for cancer subtype analysis using gene expression data.

The work consists of two complementary analyses:

1. Building and auditing a Random Forest workflow for Diffuse Large B-Cell Lymphoma (DLBCL) Cell-of-Origin (COO) prediction.
2. Identifying molecular subtypes in Esophageal Squamous Cell Carcinoma (ESCC) using unsupervised clustering and pathway analysis.

---

## Objectives

### Part 1: Supervised Learning

Develop a Random Forest workflow for DLBCL Cell-of-Origin (COO) prediction using gene expression profiles, then evaluate both threshold-independent ranking performance and threshold-dependent classification metrics.

Key objectives:

* Train and optimize a Random Forest model
* Perform feature selection to identify informative genes
* Evaluate model performance using OOB error, ROC/AUC analysis, and threshold-dependent metrics
* Externally evaluate the model on an independent validation cohort

### Part 2: Unsupervised Learning

Identify biologically meaningful molecular subtypes within ESCC samples.

Key objectives:

* Discover latent sample groups using Non-negative Matrix Factorization (NMF)
* Compare clustering approaches using Consensus Clustering
* Identify subtype-specific differentially expressed genes (DEGs)
* Characterize biological pathways associated with each subtype using GSEA

---

## Dataset

Gene expression datasets from cancer cohorts:

* Diffuse Large B-Cell Lymphoma (DLBCL)
* Esophageal Squamous Cell Carcinoma (ESCC)

Expression matrices were used as input for both supervised and unsupervised analyses.

---

## Methods

### Machine Learning

* Random Forest model development
* Hyperparameter Tuning
* Feature Selection
* ROC Curve and threshold-dependent metric analysis
* Independent Cohort Validation

### Transcriptomic Analysis

* Non-negative Matrix Factorization (NMF)
* Consensus Clustering
* Differential Expression Analysis (limma)

### Functional Enrichment

* Gene Set Enrichment Analysis (GSEA)
* Pathway Interpretation using Gene Ontology (GO)

---

## Tools and Packages

### Programming Language

* R

### Major Packages

* randomForest
* caret
* pROC
* limma
* NMF
* clusterProfiler
* Biobase
* org.Hs.eg.db

---

## Key Outcomes

### DLBCL Classification

* Developed an explicit 100-gene Random Forest workflow for COO prediction
* Performed iterative feature selection to reduce dimensionality
* Evaluated predictive performance using OOB metrics, ROC/AUC, accuracy, balanced accuracy, sensitivity, and specificity
* Identified a scientifically important distinction: the corrected external validation showed high AUC but poor default-threshold classification performance

### ESCC Subtyping

* Identified molecular subtypes using NMF clustering
* Compared clustering stability across different algorithms
* Discovered subtype-specific gene signatures
* Identified biological pathways associated with each subtype through GSEA

---

## Skills Demonstrated

### Bioinformatics

* Gene Expression Analysis
* Differential Expression Analysis
* Functional Enrichment Analysis
* Cancer Transcriptomics

### Machine Learning

* Supervised Classification
* Feature Selection
* Model Evaluation
* Hyperparameter Optimization

### Data Analysis

* Statistical Analysis
* Data Visualization
* Biological Interpretation of Results

### Research Skills

* Experimental Design
* Reproducible Analysis
* Scientific Reporting
