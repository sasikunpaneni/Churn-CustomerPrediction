# Churn Customer Prediction (Aug 2023 – Dec 2023)

Predict customer churn using EDA, feature engineering, and a Logistic Regression model.

## Key Features
- **EDA & Feature Engineering**: Identify top churn drivers.
- **Modeling**: Logistic Regression with accuracy target ~85% (on sample data).
- **Visuals**: Quick EDA plots and Tableau-ready CSVs.

## Project Structure
```
Churn-Customer-Prediction/
├── data/                      # customer_data.csv (sample) & cleaned output
├── notebooks/                 # EDA & modeling notebooks
├── outputs/                   # saved model, metrics, plots
├── scripts/                   # preprocessing, model training, viz
├── requirements.txt
├── README.md
└── LICENSE
```

## Quickstart
```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
# source .venv/bin/activate

pip install -r requirements.txt
python scripts/data_preprocessing.py
python scripts/churn_model.py
python scripts/visualization.py
```

Outputs saved to `outputs/`:
- `churn_model.pkl`
- `confusion_matrix.png`
- `feature_coefficients.csv`
- `churn_distribution.png`, `tenure_vs_churn.png`

## Tableau (Optional)
Load `data/customer_data_clean.csv` and build a dashboard for churn risk by segment.

## Tech
Python (pandas, numpy, scikit-learn, matplotlib, joblib)
