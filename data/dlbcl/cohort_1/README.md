# DLBCL Cohort 1 External Validation Data

The DLBCL cohort 1 files are required to rerun the external validation section of
`notebooks/01_dlbcl_escc_transcriptomics_analysis.Rmd`.

These `.rds` files are not tracked in GitHub because of file size and/or data
redistribution constraints. Authorized users should manually place the following
files in this directory before rerunning the external validation analysis:

```text
data/dlbcl/cohort_1/DLBCL.eSet.1.rds
data/dlbcl/cohort_1/DLBCL.eSet.2.rds
data/dlbcl/cohort_1/DLBCL.eSet.3.rds
data/dlbcl/cohort_1/DLBCL.eSet.4.rds
```

The files are expected to be Bioconductor expression objects compatible with
`Biobase::combine()`, `Biobase::exprs()`, and the `COO` phenotype field used in
the notebook.
