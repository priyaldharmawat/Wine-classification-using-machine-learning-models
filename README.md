# Wine-classification-using-machine-learning-models

Wine Quality Prediction

This project involves predicting the quality of wine based on its chemical properties using various machine learning models. It includes data preprocessing, model building, evaluation, and optimization. The models used are K-Nearest Neighbors (KNN), Decision Tree, Random Forest, Gradient Boosting, and Neural Networks.

Dataset

The dataset used is wine.csv, which contains the following key features:

Chemical properties of the wine.
quality: Target variable indicating the quality of the wine.
Unnamed: 0: Identifier column (dropped during preprocessing).

Project Workflow

1. Data Preprocessing

Checked for null values and duplicates.

Encoded the wine categorical variable using LabelEncoder.

Split the data into training and testing sets with a 70:30 ratio.

Standardized the feature data using StandardScaler.


2. Model Building and Evaluation

K-Nearest Neighbors (KNN)

Implemented KNN with varying k values (1-20).

Identified the optimal k using cross-validation and plotted an elbow curve.

Decision Tree

Built a Decision Tree model using DecisionTreeClassifier.

Evaluated accuracy, recall, and precision.

Random Forest

Built a Random Forest model using RandomForestClassifier.

Evaluated performance metrics similar to the Decision Tree model.

Gradient Boosting

Built a Gradient Boosting model using GradientBoostingClassifier.

Evaluated its performance.

Neural Networks

Implemented two neural network models with solvers adam and sgd.

Tuned hyperparameters using GridSearchCV to optimize performance.

3. Model Comparison

Compared all models based on accuracy, recall, and precision.

Visualized the comparison using bar plots.


