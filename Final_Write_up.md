## Classification Project Write-up
### Loan Defaulter Classification
#### Abstract

The goal of this project was to use classification models to predict whether the customer will be a loan defaulter or not. I worked with dataset from Kaggle along with different classification models, such as KNN, Logistic Regression, Decision Tree, Random Forest, and XGBoost, to achieve a valuable prediction. The data set is highly imbalanced so that oversampling and SMOTE were applied. After refining a model, important features are determined as well as the final testing score of the model. Overall, the model performance is lower than I expected, better data set will be collected in the future to focus more on the customer's personnel information.

#### Design

The modeling process will start with basic data cleaning and preliminary feature engineering. I classified the features into Loan information and Personal information. After training on the baseline model, more advanced models are tested. The features used are updated based on the selected final model: Random forest, due to its more balanced F1 score and Accuracy score, since the data set is highly imbalanced. 

#### Data

The data set is from [Kaggle](https://www.kaggle.com/ankitkalauni/bank-loan-defaulter-prediction-hackathon?select=train.csv). The dataset contains 67,463 points with 35 feature for each, and 9 of them are categorical. Some features that are not related are removed during the preliminary feature engineering phase. 23 of the features went into the baseline model, and in the end, 16 of the features were used in the final model.

#### Algorithms

*Feature Engineering*

1. Converting calegorical features to binary dummy variables.
2. Categorize the features into Loan informations and Personnal informations
3. Deal with imbalanced data set: SMOTE and oversampling.

*Models*
1. KNN
2. Logistic Regression
3. Random Forest
4. Decision Tree
5. XGBoost

*Evaluation*
1. Metric used: Recall, Precision, Accuracy, F1.
2. Final Results:

'F1': 0.099, 

'AUC': 0.515, 

'Accuracy': 0.914, 

'Precision': 0.104,

'Recall': 0.095

#### Tools

Numpy and Pandas for data manipulation

Scikit-learn for modeling

Matplotlib and Seaborn for plotting

#### Communication

Slides with plots.
