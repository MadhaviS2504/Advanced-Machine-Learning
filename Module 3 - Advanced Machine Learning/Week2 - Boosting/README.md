# Week 2 — Boosting

This folder contains hands-on materials for ensemble methods focused on boosting (AdaBoost, Gradient Boosting, XGBoost) and related readings.

Topics covered
- Boosting concepts: sequential ensemble learning and how boosting reduces bias
- AdaBoostClassifier and base estimator configuration
- Gradient Boosting and XGBoost (basic usage and parameters)
- Hyperparameter choices affecting boosting (learning_rate, n_estimators, max_depth)
- Data preprocessing for categorical features, train/test split, model evaluation
- Suggested reading and external resources (links and topic lists included)

Key notebooks and files
- Ensemble_Hands_On_Boosting_Notebook.ipynb — step-by-step boosting examples using the credit dataset; includes install pins and notes for Colab
- Ensemble Techiniques.docx — supporting lecture notes on ensemble techniques
- credit (1).csv — credit dataset used in the boosting examples
- Ensemble_techniques _topics  to read.txt / all python and datascicent links from youtube.txt — curated reading lists and resources

How to run
1. Open the notebook in Jupyter or Google Colab.
2. Install required packages if needed (notebook pins versions; restart kernel if you install):

```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
```

3. Run notebook cells sequentially to reproduce training, tuning, and evaluation sections.

Notes
- The boosting notebook includes an explicit pip-install cell and notes about restarting the runtime — if you change packages, restart before running later cells.
- Example results may vary depending on library versions and random seeds.
