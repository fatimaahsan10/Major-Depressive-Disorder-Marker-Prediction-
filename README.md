# MDD Biomarker Prediction from Gene Expression Data

Final Year Project — BS Biomedical Engineering, UET Lahore (2nd Position)

## Overview
End-to-end pipeline predicting Major Depressive Disorder from blood gene 
expression data, from differential expression analysis through to a 
biosensor-deployed screening tool.

## Pipeline
1. Differential gene expression analysis (GSE19738, GSE98793)
2. LASSO feature selection → 10-gene biomarker panel
3. Biological validation via STRING PPI networks, KEGG/GO enrichment
4. Benchmarked 6 classifiers (best: Logistic Regression, 78.6% accuracy, ROC-AUC 0.77)
5. Deployed on biosensor data from 30 human subjects for risk classification

## Results
[Embed your ROC curve and confusion matrix images here]

## Tools
Python, scikit-learn, XGBoost, pandas, R (bioinformatics pipeline)
