# Fairness-Aware Medical Expenditure Prediction

This project investigates the role of proxy features—attributes that indirectly encode sensitive information—in predicting medical expenditures. It emphasizes how such proxies can introduce or amplify bias, and how removing them impacts model fairness and performance.

## Project Objective

To identify and quantify the bias introduced by proxy features (e.g., race) in machine learning models used for individual medical expenditure prediction.

## Methodology

- **Dataset**: Processed survey-based medical expenditure data.
- **Features**: Demographic attributes, socioeconomic indicators, and historical spending records.
- **Models**: Regression models trained with and without proxy features.
- **Fairness Evaluation**: Subgroup-level Mean Squared Error (MSE) analysis across racial groups.
- **Proxy Detection**: Logistic regression models used to infer race from proxy variables.

## Results Summary

- Including proxy features often improves global accuracy but leads to unequal subgroup performance.
- Removing proxy features can reduce disparities but may impact overall predictive accuracy.
- The trade-off between accuracy and fairness is illustrated using subgroup MSE comparisons.

## Technical Stack

- Python
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## Repository Contents

| File              | Description                                                         |
|-------------------|---------------------------------------------------------------------|
| `Untitled-4.ipynb`| Main notebook for model training, evaluation, and fairness analysis |
| `.gitignore`      | Specifies files/folders excluded from version control               |

*Note: Dataset files (`.csv`, `.xlsx`) are excluded due to size and sensitivity.*

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/archashikamal/ml-fairness-proxy.git
   cd ml-fairness-proxy
