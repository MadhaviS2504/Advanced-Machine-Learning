# Week 3 — Model Tuning

This folder contains materials focused on model selection, cross-validation, hyperparameter tuning, and resampling for imbalanced datasets.

Topics covered
- Cross-validation techniques (K-fold CV) and why they are used
- Hyperparameter tuning using GridSearchCV and how to design search spaces
- Oversampling and undersampling strategies for class imbalance (SMOTE, random oversampling/undersampling)
- Model evaluation best practices (CV scores, confusion matrices, precision/recall for imbalanced data)
- Pipeline patterns that combine preprocessing, model, and tuning to avoid leakage

Key notebooks and files
- Hyperparameter_tuning_Notebook.ipynb — examples of GridSearch and parameter search workflows
- K_fold_cross_validation_Notebook.ipynb — demonstrations of K-fold CV and related metrics
- Oversampling_and_undersampling_Notebook.ipynb — hands-on resampling techniques for imbalanced datasets (large notebook included)
- Week 3 Overview.docx — lecture/overview notes
- MLS - Model tuning/ (supporting materials)

How to run
1. Open the notebooks in Jupyter or Google Colab.
2. Install required packages if needed:

```bash
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
```

3. Run cells sequentially. For long notebooks (oversampling notebook is large), expect longer execution time.

Notes
- Use a consistent random_state where shown to make results reproducible.
- When using oversampling methods (SMOTE, etc.), apply resampling only on the training split to avoid data leakage.
