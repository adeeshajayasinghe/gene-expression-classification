## Gene Expression Analysis Using Microarrays

This project analyzes gene expression data from the [Golub et al. (1999) dataset](https://www.kaggle.com/datasets/crawford/gene-expression) to classify leukemia samples as Acute Lymphoblastic Leukemia (ALL) or Acute Myeloid Leukemia (AML) and explore data patterns. Using 34 significant genes identified via t-test, a logistic regression model was trained for interpretable classification, and K-Means clustering was applied to group data unsupervisedly. The Jupyter notebook in this repository details the methodology and results.

- **Dataset**: 72 samples (38 training, 34 test), 7,129 genes, pre-normalized. Labels: 0 (ALL), 1 (AML).

- **Methods**:
  - **Classification**: Logistic regression with 34 genes, tuned via cross-validation.
  - **Patterns**: Gene coefficients analyzed for AML/ALL distinctions.
  - **Clustering**: K-Means (k=2) with purity evaluation.

- **Results**:
  - Logistic Regression Accuracy: 0.794
  - Top Genes: `U50136_rna1_at` (AML), `U49248_at` (ALL)
  - Clustering Purity: 0.819
