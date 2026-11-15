
# Beyond Feature Importance: Reliability and Counterfactual Consistency of XAI-Based Fairness Auditing in Automated Resume Screening

## Project Overview

This project investigates the reliability and counterfactual consistency of Explainable Artificial Intelligence (XAI)-based fairness auditing in automated resume screening.

Using the FairCVdb dataset, the study evaluates machine learning models through predictive performance, SHAP-based feature importance, explanation stability, counterfactual sensitivity, and group-wise fairness analysis.

The project uses Linear Regression and Random Forest Regressor to examine three dataset-defined prediction targets: Blind, Gender-Biased, and Ethnicity-Biased.

## Research Objectives

- Evaluate the predictive performance of Linear Regression and Random Forest Regressor.
- Examine feature contributions using SHAP explanations.
- Assess the stability of SHAP feature rankings across different random seeds and models.
- Investigate prediction sensitivity to changes in Gender and Ethnicity.
- Compare model performance across demographic groups.

## Repository Structure

```text
FairCV-XAI-Fairness-Audit/
│
├── dataset/
│
├── notebooks/
│   └── 01_Dataset_Inspection.ipynb
│
├── results/
│   ├── all_model_comparison.csv
│   ├── counterfactual_comparison.csv
│   ├── demographic_performance_gaps.csv
│   ├── ethnicity_fairness_analysis.csv
│   ├── final_project_findings.csv
│   ├── gender_fairness_analysis.csv
│   ├── linear_regression_results.csv
│   ├── shap_model_comparison.csv
│   └── strengthened_shap_findings.csv
│
├── requirements.txt
└── README.md
```

## Dataset

This project uses FairCVdb from the BiDAlab FairCVtest repository.

Original dataset repository:

https://github.com/BiDAlab/FairCVtest

Download the dataset according to the original repository's instructions and place `FairCVdb.npy` inside the `dataset` folder.

The dataset is not included in this repository.

## Technologies and Libraries

- Python
- NumPy
- Pandas
- Scikit-learn
- SHAP
- Matplotlib
- SciPy
- Jupyter Notebook

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/FairCV-XAI-Fairness-Audit.git
```

### 2. Open the project directory

```bash
cd FairCV-XAI-Fairness-Audit
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Download and place the dataset

Place the downloaded `FairCVdb.npy` file inside:

```text
dataset/FairCVdb.npy
```

### 6. Run the Jupyter Notebook

```bash
cd notebooks
jupyter notebook
```

Open `01_Dataset_Inspection.ipynb` and execute the notebook cells in order.

## Experimental Outputs

The `results` directory contains CSV files generated during the experiments, including:

- Model performance comparisons.
- SHAP model comparisons.
- Counterfactual prediction comparisons.
- Gender and ethnicity fairness analyses.
- Demographic performance gaps.
- Consolidated project findings.

## Research Scope and Limitations

This project evaluates fairness-related model behaviour using the available FairCVdb dataset. The findings are limited to the selected dataset, features, models, and experimental settings.

Counterfactual prediction changes indicate model sensitivity to modified demographic attributes; they should not independently be interpreted as proof of real-world discrimination.

## References

The dataset and experimental framework are associated with the BiDAlab FairCVtest repository. Please consult its documentation for the relevant research publications and cite the required sources when using the dataset.

## Author

Ania Rodrigues , Shruti Zore



