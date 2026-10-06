# Customer Churn Prediction

A machine learning project that predicts whether a customer is likely to **churn** (stop using a service), so a business can take action to retain them.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ayush-Raipure/customer-churn-prediction/blob/main/customer_churn_prediction.ipynb)

## Overview

Customer churn is costly, and keeping an existing customer is usually cheaper than acquiring a new one. This notebook builds a classification model that flags customers at risk of leaving, based on their account and usage data.

**Workflow:**

1. Load and explore the dataset
2. Clean the data (missing values, data types)
3. Encode categorical features and scale numerical ones
4. Split into training and test sets
5. Train classification models
6. Evaluate with accuracy, precision, recall, F1-score, and a confusion matrix
7. Identify the features that influence churn most

## Dataset

- **Source:** *(add dataset name and link, e.g. Telco Customer Churn on Kaggle)*
- **Target column:** `Churn` (Yes / No)
- **Features:** customer demographics, account information, services used, and billing details

## Tech Stack

- Python 3
- pandas, NumPy
- scikit-learn
- matplotlib / seaborn
- Jupyter Notebook / Google Colab

## Getting Started

### Run in Google Colab

Click the **Open in Colab** badge above and run all cells.

### Run locally

```bash
git clone https://github.com/Ayush-Raipure/customer-churn-prediction.git
cd customer-churn-prediction

python -m venv venv
venv\Scripts\activate        # Windows
# source venv/bin/activate   # macOS / Linux

pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

Then open `customer_churn_prediction.ipynb` and run all cells.

## Models Used

*(Edit this list to match your notebook.)*

- Logistic Regression
- Random Forest
- Decision Tree

## Results

Churn data is usually imbalanced, so look at **recall** and **F1-score** for the churn class, not just accuracy.

| Model               | Accuracy | Precision | Recall | F1-score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | -        | -         | -      | -        |
| Random Forest       | -        | -         | -      | -        |

## Possible Improvements

- Handle class imbalance with SMOTE or `class_weight="balanced"`
- Tune hyperparameters with `GridSearchCV`
- Use cross-validation for more reliable scores
- Try gradient boosting models such as XGBoost or LightGBM
- Deploy the model as a simple web app (Streamlit or Flask)

## Project Structure

```
customer-churn-prediction/
├── customer_churn_prediction.ipynb
└── README.md
```

## Author

**Ayush Raipure**
GitHub: [@Ayush-Raipure](https://github.com/Ayush-Raipure)

## License

This project is open source and available for learning and personal use.
