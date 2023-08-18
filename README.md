# Titanic Dataset Analysis

This repository contains an analysis of the Titanic dataset. The main objective is to explore the dataset, preprocess the data, and establish a relationship between different features and passenger survival.

## Contents

- Importing necessary libraries.
- Reading and combining training and testing datasets.
- Data preprocessing including:
  - Age imputation
  - Encoding categorical variables (`Sex` and `Embarked`)
  - Handling cabin data and deck assignment
- Linear regression analysis (using both scikit-learn and statsmodels).
- Visualization of relationships using Seaborn.

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `scikit-learn`: For machine learning and data modeling.
- `seaborn` and `matplotlib`: For data visualization.
- `statsmodels`: For advanced statistical models.

## Data

The primary dataset used is the Titanic dataset from Kaggle. It consists of:
- `train.csv`: Training dataset with passenger details and survival status.
- `test.csv`: Testing dataset with passenger details.

## Insights

- Gender (`Sex`), age (`Age`), and deck (`Deck`) have significant impacts on survival likelihood.
- Data visualization provides clear insights into the distribution of survival based on different features.

- ## Linear Regression Model Insights

The linear regression model was used to quantify the relationship between passenger features and survival.

- **Gender (`Sex`)**: Being female had a significant positive coefficient, suggesting that females had a higher predicted survival probability compared to males. 
  
- **Age**: The age of passengers had a negative correlation with survival, indicating that as age increased, the predicted survival likelihood slightly decreased.

- **Deck (`Deck`)**: Different deck levels, as derived from the cabin information, showed varied impacts on survival. A negative coefficient indicated that higher deck numbers (located lower in the ship) might be associated with a lower survival probability.

The model's R-squared value of 0.357 suggests that about 35.7% of the variability in survival can be explained by the model. This highlights the complexity of the survival dynamics and suggests other factors, not included in the model, also played significant roles.
