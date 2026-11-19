# Credit Risk Stats Series

Statistics and machine learning notebooks on public credit data, exploring how AI can predict loan delinquency in ways that are **accurate, explainable, and fair**.

This repository accompanies my LinkedIn series on explainable AI and responsible credit risk, and supports my doctoral research in Artificial Intelligence at the University of the Cumberlands. All analysis uses **public data only**.

## Notebooks

| # | Notebook | What it covers |
|---|----------|----------------|
| 01 | [Give Me Some Credit: Who Becomes Delinquent?](notebooks/01_give_me_some_credit_eda.ipynb) | Exploratory analysis of 150,000 borrowers: class imbalance, missing data, data quality issues, and which factors are linked to serious delinquency |

More notebooks are on the way: data cleaning, assumption checks, logistic regression in JASP and Python, model evaluation on imbalanced data, and explainable models.

## Key findings so far

- Only **6.7%** of borrowers became seriously delinquent, so accuracy alone is a misleading measure of a model.
- **19.8%** of borrowers have no reported income, and they were *less* likely to become delinquent (5.6% vs. 6.9%).
- **Past late payments** are the strongest signal: delinquency rose from about 4% for borrowers never 30–59 days late to nearly 47% for those late five or more times.

## Data

The notebooks use the **Give Me Some Credit** dataset from Kaggle. The data is subject to the competition's rules, so it is **not included** in this repository.

To run the notebooks locally:

1. Join the competition and download the data from [kaggle.com/competitions/GiveMeSomeCredit](https://www.kaggle.com/competitions/GiveMeSomeCredit/data).
2. Put `cs-training.csv` in a `data/` folder at the root of this repository.

The notebooks also run on Kaggle directly, where the data can be added as an input.

## Run it yourself

```bash
git clone https://github.com/MOHAMMEDPAYAZ/credit-risk-stats-series.git
cd credit-risk-stats-series
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Python 3.12 is recommended.

## Repository structure

```
credit-risk-stats-series/
├── notebooks/         Jupyter notebooks, numbered in series order
├── data/              Local data files (not tracked by Git)
├── requirements.txt   Python packages
└── README.md
```

## Tools

Python (pandas, NumPy, matplotlib, seaborn, scikit-learn, statsmodels), JASP, and Jupyter.

## Author

**Payaz Mohammed**, Database Administrator and PhD student in Artificial Intelligence, researching explainable, fair AI for credit unions.

- LinkedIn: [linkedin.com/in/mohammed-payaz](https://www.linkedin.com/in/mohammed-payaz/)
- Kaggle: [kaggle.com/payazmohammed](https://www.kaggle.com/payazmohammed)
- ORCID: [0009-0009-8704-6119](https://orcid.org/0009-0009-8704-6119)
- Portfolio: [mohammedpayaz.github.io/PayazMohammed_Portfolio](https://mohammedpayaz.github.io/PayazMohammed_Portfolio/)

## Data source

Credit Fusion & Kaggle. (2011). *Give Me Some Credit* [Data set]. Kaggle. https://www.kaggle.com/competitions/GiveMeSomeCredit
