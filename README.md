# Nifty50 Market Movement Prediction using Machine Learning

This project uses machine learning models to predict **market movements** in the **Nifty50 index**. The dataset contains **minute-level data (2015-2025)** to predict the next **5-minute price movement** direction using **Logistic Regression**, **Random Forest**, **XGBoost**, and **LSTM**.

## Project Overview

The goal of the project is to **predict market movements** based on **historical price patterns** and **technical indicators**. We trained various models and evaluated their performance.

### Models Used:
1. **Logistic Regression**
2. **Random Forest**
3. **XGBoost**
4. **LSTM (Long Short-Term Memory)**
   
### Key Steps:
1. **Data Preprocessing**: Cleaned the raw data and transformed it into a format suitable for model training.
2. **Feature Engineering**: Created features like **momentum**, **volatility**, **z-scores**, and **moving averages**.
3. **Model Training**: Trained multiple models on the dataset.
4. **Evaluation**: Used **accuracy**, **precision**, **recall**, **F1 score**, and **Sharpe ratio** for model evaluation.

### Challenges:
- **Market Noise**: Minute-level data is noisy and difficult to predict accurately.
- **Data Imbalance**: Most returns were small or close to zero, making predictions difficult.

### Insights:
- Predicting market movements in **short intervals** (minute-level) is inherently difficult.
- **LSTM** struggled with the noisy data, while **XGBoost** and **Random Forest** provided better, but still limited, performance.

---

## Requirements

- Python 3.6+
- Jupyter Notebook
- Libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `xgboost`
  - `tensorflow`
  - `matplotlib`
  - `seaborn`

Install all required libraries using:

```bash
pip install -r requirements.txt
