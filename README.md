# House Price Prediction using CatBoost and LightGBM

This repository contains machine learning models for house price prediction implemented using **CatBoost** and **LightGBM**.  
The complete workflow is implemented using **Jupyter Notebooks (`.ipynb`)**.

The project demonstrates data preprocessing, feature engineering, model training, hyperparameter tuning, and performance evaluation.

## Project Structure

├── CatBoost.ipynb  
├── LightGBM.ipynb  
├── requirements.txt  
├── README.md  
├── .gitignore  
└── LICENSE  

## Models Implemented

### CatBoost Regressor
- Log transformation of the target variable (`SalePrice`)
- Handling missing values for numerical and categorical features
- Ordinal encoding for categorical variables
- Feature engineering (TotalSF, Age, RemodAge, OverallQual_SF)
- Model tuning with early stopping
- Evaluation using RMSE and R² score

### LightGBM Regressor
- Log transformation of the target variable
- Handling missing values
- One-hot encoding for categorical features
- Early stopping for optimal training
- Hyperparameter tuning
- Evaluation using RMSE and R² score

## Dataset

- Dataset: **House Prices – Advanced Regression Techniques**
- Source: Kaggle

The dataset is **not included** in this repository.

Before running the notebooks, update the dataset path inside the notebooks, for example:

pd.read_csv("data/House_Price_train.csv")

## Installation

Install the required dependencies using:

pip install -r requirements.txt

## How to Run

Open the notebooks and run all cells:

- catboost.ipynb
- lightgbm.ipynb

Each notebook performs:
- Data preprocessing
- Feature engineering
- Model training
- Prediction
- Performance evaluation

## Evaluation Metrics

- RMSE (Root Mean Squared Error)
- R² Score

Both metrics are printed after model evaluation.

## Key Highlights

- End-to-end machine learning pipeline using Jupyter Notebooks
- Feature engineering and model tuning
- Early stopping to reduce overfitting
- Clean and reproducible project structure
- Suitable for academic projects and internships

## License

This project is licensed under the MIT License.
