# House Price Prediction using CatBoost and LightGBM

This repository contains machine learning models built using CatBoost and LightGBM for house price prediction.  
Both models are implemented independently and include data preprocessing, feature engineering, model training, tuning, and evaluation.

## Project Structure

.
├── catboost.py  
├── lightgbm.py  
├── requirements.txt  
├── README.md  
├── .gitignore  
└── LICENSE  

## Models Implemented

CatBoost Regressor:
- Log transformation of target variable (SalePrice)
- Handling missing values for numerical and categorical features
- Ordinal encoding for categorical variables
- Feature engineering (TotalSF, Age, RemodAge, OverallQual_SF)
- Model tuning with early stopping
- Evaluation using RMSE and R² score

LightGBM Regressor:
- Log transformation of target variable
- Missing value handling
- One-hot encoding for categorical features
- Early stopping for optimal training
- Hyperparameter tuning
- Evaluation using RMSE and R² score

## Dataset

Dataset: House Prices – Advanced Regression Techniques  
Source: Kaggle  

The dataset is not included in this repository.  
Before running the code, update the dataset path inside the scripts, for example:

pd.read_csv("data/House_Price_train.csv")

## Installation

Install the required dependencies using:

pip install -r requirements.txt

## How to Run

Run the models separately:

python catboost.py  
python lightgbm.py  

Each script performs data preprocessing, model training, prediction, and performance evaluation.

## Evaluation Metrics

- RMSE (Root Mean Squared Error)
- R² Score

Both metrics are printed after model evaluation.

## Key Highlights

- End-to-end machine learning pipeline
- Feature engineering and model tuning
- Early stopping to reduce overfitting
- Clean and reproducible project structure
- Suitable for academic projects and internships

## License

This project is licensed under the MIT License.
