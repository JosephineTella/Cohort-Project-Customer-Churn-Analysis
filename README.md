# Cohort Project: Customer Churn Analysis
The ConnectTel Customer Churn Prediction initiative aimed to build a reliable machine learning model capable of identifying customers most likely to discontinue their service. This was accomplished through a structured and comprehensive workflow that included data cleaning, exploratory data analysis (EDA), feature engineering, model experimentation, feature scaling, handling class imbalance, and systematic hyperparameter tuning. Each step was designed to improve model accuracy and strengthen the predictive power of the final solution.

### Models and Evaluation Approach
The machine learning models utilized were:
  -  XGBoost
    
  -  RandomForestClassifier
    
  -  DecisionTreeClassifier
    
  -  LogisticRegression
    
  -  SGDClassifier

Models were trained using various feature selection methods, including:

  -  RandomForest Feature Importance
    
  -  L1 (Lasso) Regularization
    
  -  Recursive Feature Elimination (RFE) 

  -  SelectKBest

  -   Mutual Information (ML)

Each model underwent hyperparameter optimization using Randomized Search to identify the best performing configuration. Performance was assessed using a held-out test set where 80% of the data was used for training and 20% for testing and model performance evaluated using four key metrics:

  -  Accuracy: overall correctness

  -  Precision: correctness of predicted churners

  -  Recall: ability to capture true churners

  -  F1 Score: the harmonic mean of precision and recall

###  Model Performance

Across most feature-selection pipelines, XGBoost consistently ranked in the top tier with:

  -  Accuracy: ~78–79%

  -  Precision: ~0.63–0.66

  -  Recall: ~0.58–0.60

  -  F1 Score: ~0.58–0.61

The top three performing models were:

  -  XGBoost + RandomForest_Importance

  -  RandomForestClassifier + RandomForest_Importance

  -  XGBoost + L1_Lasso

Among these, XGBoost + RandomForest_Importance provides the highest F1 Score and accuracy, making it the best model for churn prediction.

### Conclusion

Based on model evaluation, XGBoost is the recommended model for ConnectTel’s churn prediction pipeline. It offers the best balance of accuracy, recall, and F1 score, making it the most effective tool for driving data-informed customer retention strategies.
