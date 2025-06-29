# 🏡 House Price Prediction

Predict house prices using advanced regression techniques on the Kaggle "House Prices: Advanced Regression Techniques" dataset.

---

## 📌 Objective

To build and evaluate regression models that estimate the sale price of residential homes based on various features like square footage, location, overall quality, etc.

---

## 📂 Dataset

- Source: [Kaggle - House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- Files Used:
  - `train.csv`: Raw dataset
  - `cleaned_transformed.csv`: Cleaned & log-transformed data
  - `eda_day1_subset.csv`: Subset used during EDA

---

## 🗓️ Timeline & Tasks

| Day | Task |
|-----|------|
| 1   | EDA on features (`GrLivArea`, `Neighborhood`) |
| 2   | Handle outliers, apply log transformation |
| 3   | Train Linear Regression and Gradient Boosting models |
| 4   | Feature importance analysis and visualization |

---

## 🧪 Techniques Used

- Exploratory Data Analysis (EDA)
- Outlier detection (scatter plots, IQR)
- Log transformation to fix skewness
- One-hot encoding for categorical variables
- Linear Regression (baseline)
- Gradient Boosting Regressor (advanced model)
- Feature importance using `.feature_importances_`

---

## 🔧 Project Structure

house-price-prediction/                                                      
├── data/                                                                 
│ ├── train.csv                                                                
│ ├── cleaned_transformed.csv                                                           
│ └── eda_day1_subset.csv                                                                  
├── notebooks/                                                       
│ ├── 1_eda.ipynb                                                   
│ ├── 2_outlier_handling.ipynb                                                                     
│ ├── 3_model_training.ipynb                                                                     
│ └── 4_feature_importance.ipynb                                                                                 
├── models/                                                                                   
│ ├── linear_regression.pkl                                                                     
│ └── gradient_boosting.pkl                                                                       
├── README.md                                                                   
├── requirements.txt                                                                       
└── .gitignore                                                                              


---

## 📈 Results

| Model               | RMSE (log scale) | R² Score |
|--------------------|------------------|----------|
| Linear Regression   | ✅ ~0.17–0.18     | ✅ ~0.89  |
| Gradient Boosting   | ✅ ~0.12–0.14     | ✅ ~0.93  |

> Gradient Boosting significantly outperforms Linear Regression in both RMSE and R².

---

## 📊 Top Important Features

- `OverallQual` (Overall quality)
- `GrLivArea` (Above-ground living area)
- `GarageCars`
- `TotalBsmtSF`
- `Neighborhood_*` (location-related encoded features)

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Nitin-kandpal17/house-price-prediction.git
cd house-price-prediction
```

### 2. Create Environment
```bash
conda create -n house-price-prediction python=3.10 -y
conda activate house-price-prediction
pip install -r requirements.txt
```

### 3. Launch Jupyter
```bash
jupyter notebook
```

## ✅ To Do (Optional Enhancements)
- Add cross-validation

- Hyperparameter tuning (GridSearchCV)

- Deploy as Streamlit app

- Modularize with scripts/ folder



## 🧑‍💻 Author
Nitin Kandpal                                                                
GitHub: @Nitin-kandpal17


## 📄 License
This project is for educational and portfolio purposes only.