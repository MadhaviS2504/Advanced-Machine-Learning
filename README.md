Advanced-Machine-Learning
This repository contains course materials and hands‑on notebooks for Module 3 — Advanced Machine Learning, focusing on ensemble methods (bagging, boosting, random forests), model tuning, cross‑validation, and resampling.

Quick links

Module 3 — Advanced Machine Learning/
Week 1 — Bagging and Random Forest: Module 3 - Advanced Machine Learning/Week 1- Bagging and Random Forest/README.md
Week 2 — Boosting: Module 3 - Advanced Machine Learning/Week2 - Boosting/README.md
Week 3 — Model Tuning: Module 3 - Advanced Machine Learning/Week3 - Model Tuning/README.md
How to reproduce

git clone ... then open the Module 3 notebooks in Jupyter or Colab (instructions per-notebook).
Install the noted packages (some notebooks pin versions); restart kernel/runtime after installs.
Run cells sequentially.
Notes

Several notebooks pin package versions and include install cells — if you install packages inside a running runtime, restart before executing downstream cells.
Notebooks and datasets can be large so expect some notebooks to take time.
Expanded Week 1 README (per-notebook summaries)

Week 1 — Bagging and Random Forest
This folder contains the bagging/random-forest hands‑on materials and an additional case study.

Notebooks and what they do

Ensemble_Hands-On_Bagging-2 (1).ipynb

Loads the credit dataset, inspects distributions and types, converts object columns to categorical/ordinal codes.
Demonstrates BaggingClassifier with a chosen base estimator and RandomForestClassifier; shows when bagging reduces variance and how RF injects feature randomness.
Includes GridSearchCV examples for tuning ensemble hyperparameters, compares base learners (LogisticRegression / DecisionTree), and shows evaluation with accuracy, confusion matrix and other sklearn metrics.
Notes on reproducibility (random_state) and preprocessing to avoid leakage.
Additional Case Study/Case_Study_Diabetes_Risk_Prediction_Notebook.ipynb

Applies ensemble methods to the Pima Indians diabetes dataset: preprocessing, model training, evaluation and interpretation of results for a health-risk classification task.
Datasets

credit (2).csv — main credit dataset used across the notebooks.
Additional Case Study/pima-indians-diabetes.csv
How to run

Open in Jupyter or Colab; if necessary pip install pandas/numpy/scikit-learn/matplotlib/seaborn then run cells sequentially.
Expanded Week 2 README (per-notebook summaries)

Week 2 — Boosting
This folder contains boosting hands‑on materials plus reading lists.

Notebooks and what they do

Ensemble_Hands_On_Boosting_Notebook.ipynb
Shows how to use AdaBoostClassifier, GradientBoostingClassifier, and XGBClassifier on the credit dataset.
Contains an explicit pip-install cell with pinned versions (noted in the notebook). After install, notebook instructs to restart runtime.
Demonstrates setting a DecisionTree base_estimator with random_state when tuning AdaBoost to stabilize results.
Uses GridSearchCV to tune key hyperparameters (learning_rate, n_estimators, max_depth), compares algorithms, and evaluates with confusion matrices and standard metrics.
Includes data‑preprocessing steps for categorical features and commentary about reproducibility.
Supporting materials

Ensemble Techiniques.docx — lecture notes on ensemble concepts.
Ensemble_techniques _topics to read.txt and all python and datascicent links from youtube.txt — curated reading and video resources.
How to run

Install pinned packages (if you use the notebook cell, restart kernel after install), then run the notebook cells in order.
Expanded Week 3 README (per-notebook summaries)

Week 3 — Model Tuning
This folder focuses on model selection, cross‑validation, hyperparameter search, and handling imbalanced data.

Notebooks and what they do

Hyperparameter_tuning_Notebook.ipynb

Introduces a real‑world context (bank loss / credit default).
Shows how to design parameter grids and run GridSearchCV, including scoring choices and how to interpret cross‑validation results.
Demonstrates how to structure searches to reduce runtime and overfitting (e.g., using reasonable grid ranges and cross‑validation folds).
K_fold_cross_validation_Notebook.ipynb

Demonstrates K‑fold and StratifiedKFold, cross_val_score usage, and how to read and interpret CV statistics.
Covers repeated CV and when to prefer stratification for imbalanced classes.
Oversampling_and_undersampling_Notebook.ipynb

Hands‑on resampling: RandomOverSampler, RandomUnderSampler, and SMOTE (from imbalanced‑learn).
Shows proper placement of resampling inside a pipeline to avoid leakage, and compares evaluations with and without resampling.
Supporting materials

Week 3 Overview.docx — lecture/overview.
MLS - Model tuning/ — additional supporting files.
How to run

Install packages (pandas, numpy, scikit-learn, imbalanced-learn, matplotlib, seaborn), open notebooks, and run cells sequentially. Use pipelines and only apply resampling to training splits.
Next step If this text looks good, reply “Proceed to commit” and I will add:

The updated root README,
Expanded README.md files for Week 1, Week 2, and Week 3.
If you want edits to any paragraph, tell me which week and what to change before I commit.
