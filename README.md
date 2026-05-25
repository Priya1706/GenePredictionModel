GenePredictionModel
A machine learning project for disease prediction using biomedical datasets — built as a long-term, iterative research portfolio project.

What This Project Does
This project builds end-to-end ML pipelines that train classifiers on real biomedical datasets and evaluate their ability to predict disease status. It is designed to evolve from basic disease classification toward genomics-oriented machine learning.

Current Status
FeatureStatusData loading and cleaning pipeline✅ CompleteParkinson's disease prediction model✅ CompleteDiabetes prediction model✅ CompleteFeature importance analysis and visualization✅ CompleteMulti-model comparison (SVM, XGBoost, etc.)🔄 In ProgressAdvanced genomics dataset integration📋 PlannedDNA microarray gene expression pipeline📋 Planned

Datasets
Parkinson's Disease Dataset

Source: UCI Machine Learning Repository
Features: 23 biomedical voice measurements (jitter, shimmer, HNR, RPDE, DFA, PPE)
Target: status — 1 = Parkinson's, 0 = Healthy
Samples: 195

Pima Indians Diabetes Dataset

Source: UCI Machine Learning Repository
Features: 8 clinical measurements (Glucose, BMI, Age, BloodPressure, etc.)
Target: class — 1 = Diabetic, 0 = Non-diabetic
Samples: 768


Project Structure
GenePredictionModel/
│
├── datasets/
│   ├── parkinsons.csv
│   └── diabetes.csv
│
├── notebooks/
│   ├── parkinsons_model.ipynb    # Parkinson's prediction pipeline
│   └── diabetes_model.ipynb     # Diabetes prediction pipeline
│
├── graphs/
│   └── diabetes_feature_importance.png
│
└── README.md

How to Run
Requirements
bashpip install pandas numpy scikit-learn matplotlib jupyter
Run a notebook
bashjupyter notebook notebooks/parkinsons_model.ipynb

ML Pipeline (Both Models)

Load CSV dataset
Clean data — drop non-numeric columns, handle missing values
Encode categorical values (Yes/No → 1/0)
Split into training and test sets (80/20)
Train a RandomForestClassifier
Evaluate: accuracy, classification report, confusion matrix
Visualize feature importance


Tech Stack
ComponentTechnologyLanguagePython 3MLScikit-learnData ProcessingPandas, NumPyVisualizationMatplotlibEnvironmentJupyter NotebookVersion ControlGit & GitHub

Roadmap
Version 2 — Multi-Model Comparison

Add SVM, Logistic Regression, XGBoost, Decision Trees
Compare accuracy, precision, recall, F1-score across models
Add cross-validation and ROC curves

Version 3 — Genomics Pipeline

Integrate RSCTC 2010 DNA Microarray dataset (59,005 features, 92 samples)
Implement dimensionality reduction: PCA, SelectKBest, LASSO
Gene expression analysis and biomarker discovery


Author
Priyamvadhaa Hoskere
First-Year CSE Student — Gopalan College of Engineering and Management, Bengaluru
