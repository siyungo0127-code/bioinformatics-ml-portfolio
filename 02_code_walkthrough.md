# Code Walkthrough

## Project Overview

This project contains two major analyses:

1. DLBCL Cell-of-Origin classification using Random Forest
2. ESCC molecular subtype discovery using unsupervised clustering

The objective is to apply machine learning and transcriptomic analysis methods to understand cancer heterogeneity and identify biologically meaningful patterns.

---

# Part 1: Random Forest Classification

## Step 1. Load and Prepare Data

### Purpose

Load gene expression data and corresponding sample labels.

### Why?

Machine learning algorithms require a structured matrix where:

* Rows represent samples
* Columns represent genes
* Labels represent class membership

In this project, the target label was Cell-of-Origin (COO).

---

## Step 2. Split Training and Testing Data

### Purpose

Create independent datasets for model training and evaluation.

### Why?

Evaluating on the same data used for training can lead to over-optimistic performance estimates.

Training/Test Split:

* 70% Training
* 30% Testing

---

## Step 3. Train Random Forest Model

### Purpose

Build a classifier capable of predicting COO subtype.

### Why Random Forest?

Advantages:

* Handles high-dimensional gene expression data
* Resistant to overfitting
* Provides feature importance scores
* Performs well with noisy biological data

---

## Step 4. Hyperparameter Tuning

### Parameters Optimized

* Number of Trees (ntree)
* Number of Variables per Split (mtry)

### Purpose

Find model settings that minimize Out-of-Bag (OOB) error.

### Why?

Better hyperparameters improve prediction accuracy and generalizability.

---

## Step 5. Feature Selection

### Purpose

Reduce the number of genes used for classification.

### Why?

Gene expression datasets contain thousands of features.

Reducing feature count:

* Removes noise
* Improves interpretability
* Reduces computational complexity
* Can improve predictive performance

---

## Step 6. Evaluate Model Performance

### Metrics

* OOB Error
* ROC Curve
* AUC

### Why?

These metrics measure how well the model separates different COO subtypes.

A strong classifier should have:

* Low OOB error
* High AUC
* Consistent performance on validation data

---

## Step 7. Independent Validation

### Purpose

Test the trained model on an external cohort.

### Why?

A useful biological classifier must generalize to unseen samples.

External validation is one of the strongest indicators of model robustness.

---

# Part 2: Molecular Subtyping Using NMF

## Step 1. Perform NMF Clustering

### Purpose

Identify hidden molecular subtypes.

### Why NMF?

NMF is widely used in transcriptomics because:

* Expression values are non-negative
* Results are biologically interpretable
* Subtype discovery is often robust

---

## Step 2. Determine Optimal Number of Clusters

### Purpose

Find the most stable clustering solution.

### Why?

Too few clusters may miss biological differences.

Too many clusters may introduce noise.

The goal is to identify biologically meaningful groups.

---

## Step 3. Consensus Clustering Comparison

### Purpose

Compare NMF-derived clusters with an alternative clustering approach.

### Why?

Cluster stability is important.

Multiple clustering algorithms help assess robustness.

---

## Step 4. Differential Expression Analysis

### Method

limma

### Purpose

Identify genes that distinguish each molecular subtype.

### Why?

Subtype-specific genes provide biological insight and potential biomarkers.

---

## Step 5. Gene Set Enrichment Analysis (GSEA)

### Purpose

Identify biological pathways associated with each subtype.

### Why?

A list of genes alone is difficult to interpret.

GSEA converts gene-level information into pathway-level understanding.

Examples:

* Immune response
* Cell adhesion
* EMT-related pathways
* Metabolic processes

---

# Biological Interpretation

The discovered clusters exhibited distinct biological characteristics.

Examples include:

* Immune-related signatures
* Epithelial differentiation
* EMT-like phenotypes
* Metabolic activity

These findings suggest that the identified subtypes represent biologically meaningful disease states.

---

# Key Takeaways

This project demonstrates experience in:

* Machine Learning for Omics Data
* Random Forest Classification
* Feature Selection
* Transcriptomic Clustering
* Differential Expression Analysis
* GSEA
* Cancer Bioinformatics
* Biological Interpretation of Computational Results
