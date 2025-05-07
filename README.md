
# 📊 Credit Scoring Project

**Author**: Dauren Oralbek  
**Date**: May 2025  
**Tools**: Python, Pandas, scikit-learn, LightGBM, SHAP

---

## 🔍 Overview

This project focuses on building a credit scoring model that predicts whether an applicant is likely to repay a loan. Using anonymized customer data, we:

- Perform exploratory data analysis (EDA)
- Engineer relevant features
- Train classification models
- Evaluate performance
- Interpret results using SHAP

---

## 📁 Project Structure

```
Credit-scoring/
│
├── .venv/                   # Virtual environment
│
├── data/                    # Data files
│   ├── test.pq              # Test dataset (Parquet format)
│   └── train.pq             # Training dataset (Parquet format)
│
├── notebook/                # Jupyter notebooks
│   └── SCORING.ipynb        # Notebook for scoring
│
├── outputs/                 # Output files
│   ├── out_data.csv         # Output data in CSV format
│   └── gitattributes        # Git attributes file
│
├── .gitignore               # Git ignore file
├── CONCLUSION.md            # Conclusion documentation
├── CONTRIBUTING.md          # Contributing guidelines
├── LICENSE                  # License file
├── README.md                # Project README
└── requirements.txt         # Project dependencies
```

---

## ⚙️ How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/daurenoralbek/Credit-scoring.git
   cd Credit-scoring
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook P04_SCORING_Oralbek_Dauren.ipynb
   ```

---

## ✅ Model Performance

- Model: LightGBM Classifier
- Evaluation metric: ROC AUC Score
- Interpretability: SHAP plots for top features

---

## 📌 Key Insights

- Feature importance reveals variables like `income`, `employment status`, and `loan duration` are highly predictive.
- SHAP analysis improves trust and transparency in predictions.
- The model generalizes well across training and test data.

---

## 📜 Conclusion

You can find the written conclusion in [`Conclusion.txt`](Conclusion.txt), summarizing key business takeaways and next steps.

---

## 📄 License

This project is open-source under the [MIT License](https://opensource.org/licenses/MIT).

# 📊 Credit Scoring Project

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)


## 📂 Data Description
- `train.pq`: Training dataset with anonymized customer features (e.g., income, loan history) and target (loan repayment status).
- `test.pq`: Test dataset for generating predictions.
- Note: Data is in Parquet format for efficiency. Use `pandas.read_parquet()` to load.

## 🤝 Contributing
Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to submit issues or pull requests.
