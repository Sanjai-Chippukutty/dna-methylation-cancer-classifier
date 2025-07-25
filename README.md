# dna-methylation-cancer-classifier
This project builds a machine learning classifier using DNA methylation data to predict cancer subtypes. It processes beta values from 200 patient samples to train and evaluate classification models. The goal is to demonstrate the use of methylation biomarkers in early cancer detection.

---

📁 Dataset
Source: GEO (Gene Expression Omnibus)

Accession ID: GSE109381

Platform: Illumina HumanMethylation450 BeadChip

Samples: ~3905 (Subset of 200 used for this study)

Format: Raw IDATs and normalized Beta value tables

🎯 Objectives
Load and preprocess high-dimensional methylation profiles

Select relevant CpG features using statistical and ML-based techniques

Train classifiers (Random Forest, SVM, etc.) to predict cancer subtypes

Evaluate performance with metrics like accuracy, precision, recall, F1-score

Deploy as a Streamlit web app for interactive predictions (optional extension)

🔧 Steps & Methodology
Data Acquisition

Downloaded methylation beta matrix from GEO

Filtered 200 representative samples across subtypes

Preprocessing

Removed low-quality CpGs and samples

Normalized beta values

Encoded labels for subtype classification

Feature Selection

Variance thresholding

SelectKBest (ANOVA F-score)

Recursive Feature Elimination (RFE)

Model Training

Algorithms: Random Forest, SVM, Logistic Regression

Stratified train-test split (80/20)

5-fold Cross-validation

Evaluation

Accuracy, Confusion Matrix

ROC-AUC (if binary), Macro F1-score (for multi-class)

Visualization of feature importance and PCA

Deployment (Optional)

Streamlit interface with live input for prediction

GitHub-hosted repo with full notebook & 
