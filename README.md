# Hyperparameter Optimization for Breast Cancer Classification

## 1. Problem Formulation
- **Decision Variables (x)**: Hyperparameter vector x = [n_estimators, max_depth, min_samples_split, max_features]
- **Objective Function (f(x))**: Maximize 5-Fold Stratified Cross-Validation ROC-AUC on Training Set.
- **Constraints**: Search budget capped at 40 trials; Evaluation isolated from Test Set.
- **Baseline**: Default Scikit-Learn RandomForestClassifier parameters.
- **Optimization Method**: Optuna (Tree-structured Parzen Estimator - TPE).
