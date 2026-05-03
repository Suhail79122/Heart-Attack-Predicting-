# Heart Attack Prediction using Logistic Regression

## Overview
This project aims to predict the likelihood of heart attack occurrence using a machine learning model based on Logistic Regression. It analyzes medical and lifestyle factors to classify whether a patient is at risk or not.

## Problem Statement
Heart attacks are a major health concern worldwide. The goal of this project is to build a classification model that predicts whether a patient will experience a heart attack based on clinical and behavioral features.

## Dataset
The dataset used in this project contains various medical attributes, such as:
- Age
- Blood pressure
- Cholesterol levels
- Smoking habits
- Diabetes status
- Other health-related indicators

Target variable:
- Death Outcome (1 = Died, 0 = Survived)

## Methodology
1. Load and preprocess the dataset  
2. Handle missing values  
3. Split data into training and testing sets  
4. Apply feature scaling using StandardScaler  
5. Train a Logistic Regression model  
6. Evaluate performance using:
   - Accuracy
   - Precision
   - Recall
   - F1 Score  
7. Generate confusion matrix and classification report  
8. Visualize results using plots  

## Code

The implementation is provided in the Jupyter Notebook.

Example:

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression(max_iter=1000)
model.fit(x_train_scaled, y_train)
y_pred = model.predict(x_test_scaled)
```

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Results
The model achieved good classification performance based on evaluation metrics such as accuracy, precision, recall, and F1 score.  
The confusion matrix and classification report provide insights into model effectiveness and prediction quality.

## Visualization
The project includes:
- Confusion matrix heatmap  
- Target distribution plot  

## How to Run

1. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn notebook
```

2. Open Jupyter Notebook:
```bash
jupyter notebook
```

3. Run the project:
- Open your notebook file (e.g., `Happiness_Predictor.ipynb`)
- Run all cells 

## Future Improvements
- Use advanced classification models (Random Forest, XGBoost)  
- Improve feature engineering  
- Perform hyperparameter tuning  
- Increase dataset size for better accuracy  

## Author
Suahil – AI System Engineering Student
