# Week 1 — Bagging and Random Forest

This folder contains hands-on materials for ensemble methods focused on bagging and random forests.

Topics covered
- Bagging (Bootstrap Aggregation) and why it reduces variance
- BaggingClassifier usage and configuration
- Random Forests (RandomForestClassifier) and how they introduce feature randomness
- Using Logistic Regression / Decision Tree as base learners in ensembles
- Data preprocessing for categorical features (converting object columns to categorical/ordinal)
- Train/test split, model fitting, and evaluation using accuracy, confusion matrix and other sklearn metrics

Key notebooks and files
- Ensemble_Hands-On_Bagging-2 (1).ipynb — step-by-step Bagging and Random Forest examples using the credit dataset; includes preprocessing and model evaluation
- credit (2).csv — credit dataset used for experiments
- Additional Case Study/Case_Study_Diabetes_Risk_Prediction_Notebook.ipynb — an extra case study (diabetes risk prediction) demonstrating ensemble methods on the Pima Indians dataset
- Additional Case Study/pima-indians-diabetes.csv — dataset for the diabetes case study
- Additional Case Study/Problem Statement-Additional Case study - Week1.docx — problem statement for the extra case study

How to run
1. Open the notebook (Jupyter or Google Colab). The notebooks read `credit.csv` by default if present in the folder.
2. Install required packages (if needed):

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Run cells sequentially. The notebook converts categorical object columns to categorical/ordinal codes before training.

Notes
- Some notebooks were used in lecture and may contain inline outputs; run all cells to reproduce results.
