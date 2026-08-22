# Advanced Machine Learning — Module 3

Concise, hands‑on materials for Module 3: advanced ensemble methods and model tuning. This repository collects lecture notebooks, supporting documents, and datasets so students and practitioners can reproduce the in-class examples and run the provided case studies.

## What you'll find
- Week 1 — Bagging & Random Forests
  - Practical notebook showing BaggingClassifier and RandomForestClassifier on a credit dataset, data preprocessing for categorical features, basic hyperparameter tuning and evaluation. (See: Module 3 - Advanced Machine Learning/Week 1- Bagging and Random Forest/README.md)
- Week 2 — Boosting
  - Hands-on notebook covering AdaBoost, Gradient Boosting and XGBoost, with tips for tuning learning_rate, n_estimators and max_depth. Includes curated reading lists. (See: Module 3 - Advanced Machine Learning/Week2 - Boosting/README.md)
- Week 3 — Model Tuning
  - Notebooks on K‑fold cross validation, GridSearchCV, and resampling for imbalanced data (SMOTE, oversampling/undersampling). Includes guidance on pipelines and avoiding data leakage. (See: Module 3 - Advanced Machine Learning/Week3 - Model Tuning/README.md)
- Project folder
  - EasyVisa case study notebook (.ipynb and exported .html) and dataset; an end‑to‑end example applying the techniques from the module.

## Quick start
1. Clone the repository:

```bash
git clone https://github.com/MadhaviS2504/Advanced-Machine-Learning.git
cd "Advanced-Machine-Learning/Module 3 - Advanced Machine Learning"
```

2. Open a notebook in Jupyter or upload the .ipynb to Google Colab.
3. Install dependencies if needed (some notebooks pin versions):

```bash
# common packages used across notebooks
pip install pandas numpy scikit-learn matplotlib seaborn
# for boosting notebooks
pip install xgboost
# for resampling notebooks
pip install imbalanced-learn
```

4. If you run pip installs inside a running runtime (e.g., Colab), restart the kernel/runtime before executing subsequent cells.
5. Run cells sequentially in each notebook to reproduce the analyses.

## Highlights — what to try first
- Week 1: open `Ensemble_Hands-On_Bagging-2 (1).ipynb` to see preprocessing + Bagging vs Random Forest comparisons.
- Week 2: open `Ensemble_Hands_On_Boosting_Notebook.ipynb` (contains an install cell with pinned versions and notes about restarting the runtime).
- Project: open `Project/Case_Study_EasyVisa_Prediction_Notebook (4).ipynb` for an end‑to‑end case study using the supplied CSV.

## Reproducibility notes
- Several notebooks pin package versions (especially the boosting notebook). If you change installed packages, restart the kernel/runtime before running downstream cells.
- Use the shown `random_state` values where provided to make experiments deterministic.
- Always fit resampling (SMOTE / oversampling) only on the training split — many notebooks demonstrate correct placement via sklearn Pipelines.

## File map (top-level)
- `Module 3 - Advanced Machine Learning/`
  - `Week 1- Bagging and Random Forest/`
  - `Week2 - Boosting/`
  - `Week3 - Model Tuning/`
  - `Project/` — EasyVisa case study and dataset

## Questions or contributions
If you find issues, want clearer instructions for a notebook, or want an environment file (requirements.txt / environment.yml) created from the notebooks, open an issue or comment on the repository.

---
Updated README to provide an organized, beginner‑friendly overview of Module 3 materials and clear steps to reproduce the notebooks.
