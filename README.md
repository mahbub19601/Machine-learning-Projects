# 🚀 Machine Learning Projects: Regression and Classification
This repository contains two distinct machine learning projects: a regression task to predict housing prices and a classification task to predict Titanic survival. Both projects follow a full machine learning pipeline, from data preprocessing and feature engineering to model training and evaluation.

# 🏡 Regression Project: Housing Price Prediction
This project focuses on predicting median house values using a housing dataset. It demonstrates a systematic approach to handling numerical data, skewed distributions, and categorical features.

# Key Steps & Findings:

Data Cleaning: We started with a dataset of 1,000 samples and removed 19 rows with missing values, leaving 981 samples for the analysis.


Feature Engineering: To improve model performance, we:

Applied 

logarithmic transformations to skewed features like total_rooms and population to stabilize their variance.


Created new 

ratio-based features, such as bedroom_ratio (total bedrooms to total rooms) and household.rooms (total rooms to households).


Used 

one-hot encoding to convert the categorical ocean_proximity feature into dummy variables.

Model Performance: We compared several regression models, including Linear Regression, Decision Tree, Random Forest, and Gradient Boosting.

The 

ensemble methods (Random Forest and Gradient Boosting) significantly outperformed the simpler baseline models.


Gradient Boosting achieved the best performance with an R 
2
  of 0.68, while our main model, Random Forest, followed closely with an R 
2
  of 0.67.

The feature importance analysis showed that 

median_income was the most critical factor in predicting house values.


🚢 Classification Project: Titanic Survival Prediction
This project tackles the classic Titanic dataset to predict whether a passenger survived. It highlights the importance of thoughtful data imputation and feature scaling for classification tasks.

Key Steps & Findings:

Data Preprocessing: We handled missing data by imputing the Age column using the mean age specific to each passenger class (Pclass). Irrelevant columns like 

Name and Ticket No. were dropped.

Feature Engineering & Scaling:

Categorical variables like 

Sex and Embarked were one-hot encoded to be used by the algorithms.

All numerical features were 

scaled using MinMaxScaler to ensure no single feature disproportionately influences the models.

Model Performance: We evaluated multiple classifiers, including SVM, Logistic Regression, KNN, Decision Tree, and Random Forest.

The 

Random Forest classifier was the top performer, with an overall accuracy of 87% and a strong, balanced recall for survivors (0.82).


The Decision Tree also performed well, achieving 

85% accuracy.

The analysis demonstrated how ensemble methods can effectively handle datasets with mixed numerical and categorical features.

🤖 Conclusion
This work illustrates the power of methodical data preparation and the use of ensemble-based models. These techniques consistently led to superior predictive outcomes in both regression and classification tasks, outperforming simpler, un-tuned baselines.
