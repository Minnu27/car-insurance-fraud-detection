# car-insurance-fraud-detection

Overview
This project aims to detect fraudulent insurance claims using machine learning techniques. The dataset used for this task is sourced from Kaggle and contains various features related to insurance claims. The primary objective is to classify claims as fraudulent or authentic using supervised classification methods.

Project Structure

Data Gathering and Preparation
Data Analysis and Visualization
Explanatory Model Building
Predictive Model Building
Dataset
Source: Kaggle Auto Insurance Claims Data
Features: Includes policy details, claims amounts, customer information, and incident specifics.
Steps and Methodology
1. Data Gathering and Preparation
Loading the Data: The dataset is read into a pandas DataFrame.
Data Cleaning:
Dropping irrelevant columns.
Deriving new features such as the months between policy bind date and incident date.
Handling erroneous data, duplicates, and missing values.
Outlier Detection and Treatment: Utilizing box plots, Z-scores, and IQR methods to identify and treat outliers.
2. Data Analysis and Visualization
Exploratory Data Analysis (EDA): Visualizations to understand the distribution of fraud vs. non-fraud claims across significant features.
Correlation Analysis: Heatmaps to identify feature correlations, leading to informed feature selection.
3. Explanatory Model Building
Model Training: Training multiple machine learning models including:
Logistic Regression
K-Nearest Neighbors
Gaussian Naive Bayes
Decision Trees
Random Forest
XGBoost
Model Evaluation: Using metrics like accuracy, precision, recall, and F1-score to evaluate model performance.
4. Predictive Model Building
Handling Imbalanced Data:
Implementing techniques like SMOTE, Tomek links, and ADASYN to create a balanced dataset.
Hyperparameter Tuning: Using GridSearchCV to find optimal parameters for the XGBoost model.
Threshold Optimization: Determining the best probability threshold for classification using the ROC curve.

Final Results
The project culminates in the selection of the XGBoost classifier, optimized through hyperparameter tuning and evaluated against an optimal threshold. The final model's performance metrics are as follows:

Precision: 0.96
Recall: 0.81
F1-Score: 0.88
Accuracy: 0.83
Technologies Used
Python: Pandas, NumPy, Scikit-learn, XGBoost, Imbalanced-learn
Visualization: Matplotlib, Seaborn, SHAP for feature importance analysis

Conclusion
This project demonstrates a comprehensive approach to fraud detection in car insurance claims through data preparation, analysis, and model building. The final model shows strong predictive performance, making it a valuable tool for identifying fraudulent claims.
