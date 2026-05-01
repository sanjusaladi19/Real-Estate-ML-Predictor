# Real-Estate-ML-Predictor
Engine
📌 Project Overview
This project develops a predictive model to estimate residential house prices in Ames, Iowa. Using Lasso Regression, the engine analyzes over 70 features—ranging from lot size to neighborhood quality—to provide accurate valuations.

The goal was to create a "smart" model that doesn't just predict price, but identifies the key drivers that increase property value.

📊 Business Insights
Through Feature Importance analysis, the model revealed that the top 3 drivers of house value in this dataset are:

Overall Quality: The material and finish of the house.

Above Ground Living Area: Total square footage.

Neighborhood: Specific locations like Northridge Heights command a significant premium.

🛠️ Technical Workflow
1. Data Cleaning & Preprocessing
Outlier Removal: Houses with >4,000 sq. ft. were removed to prevent the model from being skewed by "mansion" outliers.

Missing Data: Handled null values by imputing medians for numerical data and "None" for categorical features (indicating the absence of a feature like a pool or basement).

Feature Encoding: Used One-Hot Encoding to convert categorical variables into a format suitable for linear algebra.

2. Modeling: Why Lasso Regression?
I implemented Lasso (L1 Regularization) to:

Prevent Overfitting: By penalizing complex models.

Automatic Feature Selection: Lasso successfully "zeroed out" irrelevant features, simplifying the model while maintaining high accuracy.

3. Evaluation Metrics
R² Score: 0.873 (The model explains 87% of the price variance).

Mean Absolute Error (MAE): 18588.6 (Average deviation from actual price).
