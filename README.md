# Heart Disease Classification -- Machine Learning Project

## Author

GitHub Username: Mannx22\
Contact Email: mannpatelex@gmail.com

------------------------------------------------------------------------

## Overview

This repository contains the implementation for **Problem Set #1:
Classification with Tabular Data**.

The objective of this project is to evaluate whether supervised machine
learning models can accurately predict the presence of heart disease
using structured clinical and demographic data.

Two models are compared: - Logistic Regression\
- Random Forest

Logistic Regression was selected as the final model based on superior
test-set performance.

------------------------------------------------------------------------

## Research Question

Can supervised classification models reliably predict heart disease
status based on patient medical indicators?

------------------------------------------------------------------------

## Dataset

The dataset consists of 303 patient observations and 14 variables.

Target variable: - `target`\
- 0 = No heart disease\
- 1 = Heart disease

Feature categories:

**Numerical Variables** - age\
- trestbps\
- chol\
- thalach\
- oldpeak

**Categorical Variables** - sex\
- cp\
- fbs\
- restecg\
- exang\
- slope\
- ca\
- thal

The dataset contains no missing values.

------------------------------------------------------------------------

## Methodology

### Data Preparation

-   80/20 stratified train-test split\
-   One-hot encoding for categorical variables\
-   Standard scaling for numerical variables (Logistic Regression)\
-   5-fold cross-validation\
-   ROC-AUC as optimisation metric

### Models Evaluated

**Logistic Regression** - L2 regularisation\
- Hyperparameter tuning for C

**Random Forest** - Tuned number of trees\
- Tuned maximum depth\
- Regularised split parameters

------------------------------------------------------------------------

## Evaluation Metrics

-   Accuracy\
-   Precision\
-   Recall\
-   F1-score\
-   ROC-AUC\
-   Confusion Matrix\
-   ROC Curve\
-   Precision--Recall Curve

------------------------------------------------------------------------

## Final Model Performance

  Model                 Accuracy   ROC-AUC
  --------------------- ---------- ---------
  Logistic Regression   0.885      0.910
  Random Forest         0.770      0.903

Logistic Regression demonstrated stronger generalisation performance and
was selected as the final model.

------------------------------------------------------------------------

## Project Structure

    heart-disease-classification/
    │
    ├── heart.csv
    ├── heart_disease_analysis.ipynb
    ├── requirements.txt
    └── README.md

------------------------------------------------------------------------

## How to Reproduce

1.  Clone the repository:

```{=html}
<!-- -->
```
    git clone https://github.com/Mannx22/heart-disease-classification.git
    cd heart-disease-classification

2.  Install dependencies:

```{=html}
<!-- -->
```
    pip install -r requirements.txt

3.  Open the notebook and run all cells sequentially.

------------------------------------------------------------------------

## Required Libraries

-   pandas\
-   numpy\
-   scikit-learn\
-   matplotlib\
-   seaborn

------------------------------------------------------------------------

## Reproducibility

-   Fixed random seed used\
-   Cross-validation applied\
-   Fully commented code\
-   All preprocessing steps included in pipelines

------------------------------------------------------------------------

## Limitations

-   Small dataset (303 observations)\
-   No external validation\
-   Predictive modelling only (no causal inference)

------------------------------------------------------------------------

This project was developed for academic coursework purposes.
