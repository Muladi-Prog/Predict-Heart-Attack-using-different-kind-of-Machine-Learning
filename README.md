# Predict-Heart-Attack-using-different-kind-of-Machine-Learning
Trying to figure out which the best Machine Learning method to predict heart attack
==================================================================================
Experimented with three algorithms: Logistic Regression, Support Vector
Machine, and K-Nearest Neighbor Algorithm. We scaled data using 2 scalers that are
MinMaxScaler and StandardScaler. And then we specify our input data based on 4
category
- normal input
- selected feature using Principal Component Analysis (PCA)
- 5 most important feature based on XGB (Extreme Gradient Boost algorithm)
- 5 most important feature based feature correlations
And then we show our accuracy based on the regular prediction and cross-validation
with 5 folds.
- Our data is clean so we don’t need to do data cleaning.
- For data scaling, we use 2 scalers that are min-max scaler and standard scaler.
1) Min Max Scaler
Scales date between 0 and 1 based on the minimum and maximum data.
2) Standard Scaler
Process data by reducing all data by mean then divide it by standard deviation
from data collection.
Our steps :
1. Split our data into feature and target with 80% for training and 20% for testing
2. Make 4 types of feature that is:
a. Normal input (all column)
b. PCA (principal component analysis) with 2 selected components
c. feature importance based on XGBoost (5 feature)
We take the highest feature importance it is cp, ca, sex, thal, and old peak
d. feature correlation (the most 5 correlated features)
We take the feature that has more than 0.3 correlation.
ca ,oldpeak, cp, thalach dan exang
3. Make the experiment based on 2 scalers (min-max and standard scaler and try to
decide which scalers are the best. More details in our experiment table.
4. Make the experiment into 3 model machine learning(Logistic Regression, KNN,
SVM), and try to get the best model that delivers the highest accuracy. More detail
in our table experiment.
5. Predict the model using cross-validation using 5 folds to prevent overfitting.
6. Note the accuracy model experiments.
