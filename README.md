# CreditWise-Loan-System

A Machine Learning project that analyzes applicant financial profiles and predicts loan approval outcomes using classification algorithms.

## Overview

CreditWise explores how financial and demographic attributes influence loan approval decisions. The project implements an end-to-end machine learning workflow, covering data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation.

**Objective:** Develop and compare classification models to predict whether a loan application is likely to be approved or rejected.

## Tech Stack

- **Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Environment:** Jupyter Notebook

## Dataset

The dataset contains **1,000 applicant records and 20 attributes**, including:

- Financial: Applicant Income, Co-applicant Income, Savings, Loan Amount.
- Credit Profile: Credit Score, Existing Loans, DTI Ratio.
- Personal: Age, Dependents, Marital Status, Education Level.
- Employment: Employment Status, Employer Category.
- Target: `Loan_Approved` (Yes/No).

## Methodology

The project follows these steps:

1. **Data Exploration:** Examined dataset structure, statistical summaries, distributions, and missing values.
2. **Data Preprocessing:** Handled missing values using mean and mode imputation.
3. **Exploratory Data Analysis:** Investigated feature distributions, outliers, and relationships with loan approval.
4. **Feature Engineering:** Applied Label Encoding, One-Hot Encoding, and polynomial feature transformations.
5. **Feature Scaling:** Standardized features using `StandardScaler`.
6. **Model Development:** Trained and compared three classification algorithms.
7. **Evaluation:** Assessed model performance using accuracy, precision, recall, F1-score, and confusion matrices.

## Models & Results

Three classification algorithms were evaluated:

| Model | Initial Accuracy | After Feature Engineering |
|---|---:|---:|
| Logistic Regression | 86.50% | **88.00%** |
| K-Nearest Neighbors | 76.00% | 78.50% |
| Gaussian Naive Bayes | 86.50% | 86.00% |

**Key Result:** Logistic Regression achieved the highest recorded accuracy of 88% after feature engineering, compared to 86.50% in the initial experiment.

*Note: These are experimental results from the current notebook and have not yet been independently validated against preprocessing leakage.*

## Repository Structure

```text
CreditWise-Loan-System/
│
├── credit_wise.ipynb
├── loan_approval_data.csv
├── README.md
└── .gitignore
```

## Getting Started

**1. Clone the repository**

```bash
git clone https://github.com/RiyaPadwalkar/CreditWise-Loan-System.git
```

**2. Navigate to the project directory**

```bash
cd CreditWise-Loan-System
```

**3. Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**4. Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `credit_wise.ipynb` and execute the cells sequentially. Ensure the dataset is present in the project directory.


---

**Developed using Python, Pandas, and Scikit-learn.**
