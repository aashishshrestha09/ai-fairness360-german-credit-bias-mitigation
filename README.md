# AI Fairness 360 - German Credit Bias Mitigation

## Project Overview

This project demonstrates bias detection and mitigation in the German Credit dataset using IBM's AI Fairness 360 (AIF360) toolkit. It analyzes fairness considerations in credit approval decisions across different demographic groups and saves reproducible artifacts (CSV summary and comparison screenshot).

## Project Structure

```text
├── README.md
├── requirements.txt
├── notebooks/
│   └── german_credit_bias_analysis.ipynb
└── results/
    ├── german_credit_fairness_summary.csv
    └── screenshots/
        └── fairness_metrics_comparison.png
```

## Setup Instructions

### 1. Create and Activate Virtual Environment (Python)

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 2. Register Jupyter Kernel (optional)

```bash
python -m ipykernel install --user --name uc-aif360-311 --display-name "Python (UC AIF360 venv)"
```

### 3. Run Analysis

```bash
jupyter notebook notebooks/german_credit_bias_analysis.ipynb
```

Artifacts produced:

- `results/german_credit_fairness_summary.csv`
- `results/screenshots/fairness_metrics_comparison.png`

## Key Concepts

### Fairness Metrics

- **Disparate Impact**: Ratio of favorable outcomes between unprivileged and privileged groups
- **Statistical Parity Difference**: Difference in selection rates between groups
- **Equal Opportunity Difference**: Difference in true positive rates
- **Average Odds Difference**: Average of differences in FPR and TPR

### Protected Attributes

- Age (< 25 vs >= 25) [used in this analysis]
