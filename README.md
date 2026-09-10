# Diabetes Prediction ML Project

A binary-classification notebook that predicts diabetes outcomes from common clinical measurements. It walks through data inspection, preprocessing, baseline training, model comparison, and evaluation with both threshold-based and ranking metrics.

> This repository is an educational demonstration, not medical advice or a clinically validated diagnostic system.

## Workflow

- Explore distributions, missing or implausible zero values, and feature relationships.
- Separate the `Outcome` target from the diagnostic measurements.
- Create reproducible training and test sets.
- Standardize features for logistic regression.
- Evaluate with accuracy, precision, recall, F1, confusion matrix, classification report, and ROC AUC.
- Compare logistic regression, a bounded-depth decision tree, and random forest.

## Dataset

`diabetes_dataset.csv` contains 767 patient records with the following predictors: pregnancies, glucose, blood pressure, skin thickness, insulin, BMI, diabetes pedigree function, and age. `Outcome` is the binary target.

## Repository contents

| File | Purpose |
| --- | --- |
| `Diabetes_Predictor.ipynb` | Complete exploratory and modeling workflow |
| `diabetes_dataset.csv` | Source dataset |

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install jupyter numpy pandas matplotlib seaborn scikit-learn
jupyter lab Diabetes_Predictor.ipynb
```

Run the notebook cells sequentially so that cleaning and preprocessing are applied before model evaluation.
