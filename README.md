# Credit-Card-Fraud-Detection
A machine learning project that detects fraudulent credit card transactions using Random Forest classification. Achieved 95.29% ROC-AUC score with excellent precision and recall metrics.

## Project Overview
Credit card fraud is a significant problem in the financial industry. This project implements a machine learning solution to automatically identify potentially fraudulent transactions, helping financial institutions protect their customers and reduces losses.

## Dataset
The dataset contains transactions made by credit cards in Septemeber 2013 by European cardholdrs. It presents transactions that occured in two days, where we have 492 frauds out of 284,807 transactions

## Key Features:
1. 284,807 transactions
2. 492 fraud cases (0.17% of all transactions)
3. 30 features (V1-V28 are PCA transformed, Time, Amount and class)
4. Highly imbalanced dataset

## Technologies Used
Pandas - Data manipulation and analysis
Numpy- Numerical computing
Scikit-learn - Machine Learning algorithms.
Matplotlib and Seaborn - Data visualisation
Random Forest Classifier - Main algorithm

### Model Performance
Results Achieved:
1. ROC-AUC Score:95.29%
2. Precision:96%(Class1 - Fraud)
3. Recall: 74% (Class1 - Fraud)
4. F1-Score: 84% (Class1 - Fraud)
5. Overall Accuracy:100%

## Confusion Matrix:
   [[56861      3]
    [   25     731]]
## Keys Insights :
1. Successfully identified 731 out of 756 actual fraud cases
2. Only 3 false positives out of 56,864 legitimate transactions.
3. Model handles class imbalance effectively using class_weight='balanced'

## Methodology
1. Data Exploration: Analyzed class distribution and basic statistics
2. Data Preprocessing: Features were already scaled (PCA transformed)
3. Model Selection: Random Forest Classifier chosen for:
  - Handling imbalanced datasets well
  - Feature importance insights
  - Robust performance without extensive hyperparameter tuning
4. Evaluation: Used stratified train test split and multiple metrics
5. Class Balancing: Applied class_weight='balanced' to handle imbalanced data.

## Feature Importance
The model provides insights into which features are most important for fraud detection. Feature importance analysis helps understand the decision-making process and can guide feature engineering efforts.

## Key Features
1. Imbalanced Data Handling: Uses class weighting to address the 99.83% vs 0.17% class distribution
2. Comprehensive Evaluation: Multiple metrics including confusion matrix, classification report and ROC-AUC
3. Feature Analysis: Identifies most important features for fraud detection
4. Visualization: Clear plots showing class distribution and feature importance

### Business Impact
1. Cost Reduction: Minimizes financial losses from fraudulent transactions.
2. Customer Protection : Helps protect customers from unauthorized charges.
3. Operational efficiency: Automate fraud detection process.
4. Risk Management:Provides probability scores for transaction risk assessment.

### Future Improvements:
1. Implement cross- validation for more robust performance estimation.
2. Try ensemble methods(XGBoost, LightGBM)
3. Feature engineering on Time and Amount Variables
4. Implement real time prediction API
5. Add more sophisticated evaluation metrics for imbalnced datasets
6. Hyperparameter tuning using GridSearch or RandomSearch

### Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## Contact
Email : wisdomokparaji@gmail.com
LinkedIn : Okparaji Wisdom
    
7. 
8. 
