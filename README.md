# MDD Biomarker Prediction from Gene Expression Data

Final Year Project — BS Biomedical Engineering, University of Engineering and Technology, Lahore (2nd Position)

## Overview

End-to-end pipeline predicting Major Depressive Disorder from blood gene
expression data, from differential expression analysis through to a
biosensor-deployed screening tool.

## Pipeline

1. Differential gene expression analysis on public transcriptomic datasets
2. LASSO feature selection → 10-gene biomarker panel (CABIN1, FCN2, ADK, GTPBP6, CD86, NDRG1, PMP22, PPP6C, DR1, GYG1)
3. Biological validation via STRING PPI networks, CytoHubba hub-gene ranking, and KEGG/GO pathway enrichment
4. Benchmarked 6 classifiers (Logistic Regression, SVM, Random Forest, ANN, LDA, XGBoost) with 5-fold cross-validation
5. Deployed the trained model on biosensor data from 30 human subjects for MDD risk classification (High Risk / Normal)

## Results

Best model: **Logistic Regression — 78.6% accuracy, ROC-AUC 0.77**

![ROC Curve](roc%20curve.png)

![Confusion Matrix](confusion%20matrix.png)

![Cross Validation](cross%20validation.png)

![R2, RMSE, MAE Values](R2%20score%2C%20RMSE%20value%2C%20MAE%20values.png)

## Data

Public gene expression datasets from NCBI GEO:
- [GSE19738](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE19738)
- [GSE98793](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE98793)

## Tools & Environment

- Python 3, run in Google Colab
- Libraries: scikit-learn, XGBoost, pandas, NumPy, SciPy, matplotlib, seaborn
- R (RStudio) for bioinformatics pipeline: batch correction, STRING/Cytoscape network analysis, KEGG/GO enrichment

## Hardware

Trained model deployed against biosensor-collected data from 30 human subjects for real-world risk classification.
