This repository contains a **single Jupyter notebook** implementing a full pipeline for predicting house sale prices on the Ames Housing dataset using a linear model (Ridge Regression).

## 📦 Project Structure

```
Ames-House-pricing/
├── data/                  # Raw dataset files (train.csv, test.csv)
├── Submission / 
├── Ames_house_prediction.ipynb       # Your main Kaggle-exported notebook
├── requirements.txt       # Python dependencies               
└── README.md              # Project overview and instructions
```

## 🚀 Getting Started

1. **Clone the repo**

   ```bash
   git clone https://github.com/Sirvikkaz/Ames-House-pricing.git
   cd Ames-House-pricing
   ```
2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```
3. **Launch the notebook**

   ```bash
   jupyter lab notebooks/Ames_house_prediction.ipynb
   ```

## 🔍 Notebook Overview

* **EDA & Cleaning:** Outlier detection and pruning, missing value handling
* **Feature Engineering:** Scaling numeric features, encoding categoricals, target transform
* **Modeling:** Ridge Regression (α=3) with cross-validation
* **Evaluation:** Train & validation metrics (RMSE, R²), Kaggle RMSLE metric

## 📈 Results

* **Best Model:** Ridge Regression (α=3)
* **Validation Performance:**

  * RMSE (price): $15,935
  * R²: 0.939
  * RMSLE (log price): 0.11

## 🎯 Next Steps

* Test **tree‑based models** (LightGBM, XGBoost) and compare performance
* Modularize code into `src/` for cleaner reuse
* Add **neural network** experiments
* Share insights and plots in a final report or slide deck

---

© Olanrewaju, Victor 2025
