# BCGX_PowerCo Churn Prediction Project

<!-- C:\Users\mvidal1\Desktop -->

## Project Overview

This project is focused on predicting customer churn for PowerCo, a utility company. The primary objective is to build a robust machine learning model that can accurately predict which customers are likely to leave the company, enabling proactive retention strategies.

## Dataset

- **Source:** The dataset for this project was downloaded from Kaggle via [The Forage Virtual Experience Program](https://www.theforage.com/virtual-experience/Tcz8gTtprzAS4xSoK/bcg/data-science-ccdz/business-understanding-hypothesis-framing).
- **Features:** The dataset includes various customer attributes such as usage patterns, demographic information, and service subscription details.
- **Target:** The target variable is binary, indicating whether a customer has churned (1) or not (0).

## Tools & Libraries Used

- **Data Analysis:**
  - `Matplotlib` (Graphic plot)
  - `Groupby()`
  - `info()`
  - `duplicated()`
  - `isnull()`
  - `describe()`
- **Data Transformation:**
  - `OrdinalEncoder()` for transforming categorical variables into numerical values
- **Data Visualization:**
  - `seaborn.heatmap()` for plotting dataset correlations
- **Data Preprocessing:**
  - `sklearn MinMaxScaler` for data normalization
  - `sklearn.utils shuffle` for shuffling the data
- **Model Training:**
  - `LogisticRegression`
  - `XGBClassifier`
  - `CatBoostClassifier`
  - `DecisionTreeClassifier`
  - `GradientBoostingClassifier`
  - `KNeighborsClassifier`
  - `RandomForestClassifier`
- **Model Evaluation:**
  - `confusion_matrix`
  - `classification_report`
  - `precision_score`
  - `recall_score`
  - `f1_score`
  - `accuracy_score`

## Methodology

1. **Data Exploration:** 
   - Performed exploratory data analysis (EDA) to understand the dataset's structure and key patterns.
   - Identified and handled missing values and duplicates.

2. **Feature Engineering:**
   - Converted categorical variables to numeric using `OrdinalEncoder()`.
   - Visualized feature correlations with a heatmap to guide feature selection.

3. **Data Splitting:**
   - Split the dataset into training, validation, and test sets to evaluate model performance.

4. **Model Training:**
   - Trained seven different algorithms to identify the best-performing model.
   - The models were evaluated using various metrics, with `RandomForestClassifier` showing the best performance.

5. **Model Evaluation:**
   - Achieved an accuracy of **90%** with the `RandomForestClassifier`.
   - Generated evaluation metrics such as confusion matrix, classification report, and F1 score to assess model performance.

## Results

- The `RandomForestClassifier` outperformed other models, achieving a 90% accuracy rate on the test data.
- The model's precision, recall, and F1 score indicated a balanced performance in predicting both churned and non-churned customers.

## Conclusion

The project successfully developed a machine learning model with high accuracy for predicting customer churn at PowerCo. The insights gained from this analysis can be leveraged to implement effective customer retention strategies.

## Future Work

- Experiment with hyperparameter tuning to further improve model performance.
- Explore additional feature engineering techniques to enhance the predictive power of the model.
- Consider deploying the model as a web application for real-time churn prediction.

