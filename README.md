# Happiness Predictor using Linear Regression

## Overview
This project aims to predict people's happiness scores using a machine learning model based on Linear Regression. It analyzes socio-economic factors to understand their impact on overall life satisfaction.

## Problem Statement
Happiness is influenced by various economic and social indicators. The goal of this project is to build a predictive model that estimates happiness scores based on measurable features.

## Dataset
The dataset used in this project is included in this repository:

- `2020.csv`

It contains features such as:
- GDP per capita
- Social support
- Healthy life expectancy
- Freedom to make life choices
- Generosity
- Perceptions of corruption

Target variable:
- Happiness Score

## Methodology
1. Load and preprocess the dataset  
2. Select features and target variable  
3. Split data into training and testing sets  
4. Train a Linear Regression model  
5. Evaluate performance using:
   - MAE
   - MSE
   - RMSE
   - R² Score  
6. Visualize actual vs predicted values  

## Code

The implementation is provided in the Jupyter Notebook:

- `Happiness_Predictor.ipynb`

Example:

```python
import pandas as pd
from sklearn.linear_model import LinearRegression

df = pd.read_csv("2020.csv")

X = df[[
    "GDP per capita",
    "Social support",
    "Healthy life expectancy",
    "Freedom to make life choices",
    "Generosity",
    "Perceptions of corruption"
]]
y = df["Score"]

model = LinearRegression()
model.fit(X, y)
```

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## Results
The model achieved good performance based on evaluation metrics such as MAE, MSE, RMSE, and R² score.  
The visualization of actual vs predicted values shows a strong correlation, indicating that the model fits the data reasonably well.

## How to Run

1. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib notebook
```

2. Open Jupyter Notebook:
```bash
jupyter notebook
```

3. Run the project:
- Open `Happiness_Predictor.ipynb`
- Run all cells

## Future Improvements
- Apply advanced models such as Random Forest or XGBoost  
- Improve feature selection and preprocessing  
- Optimize model performance  
- Add interactive visualization  

## Author
Suhail – AI System Engineering Student
