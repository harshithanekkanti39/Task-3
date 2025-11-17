# Task-3

Objective

The goal of this task is to build, train, and evaluate a Linear Regression model using the Titanic Dataset.
This includes cleaning the data, encoding categorical features, scaling values, analyzing correlations, and training a regression model to predict the Fare of a passenger.

Dataset Used
titanic.csv

Steps Performed
1. Import & Explore the Dataset

Loaded dataset using Pandas

Displayed head(), info(), describe()

Checked datatype of all features

Data Cleaning

Performed essential cleaning steps:

Feature	Action
Age	Filled missing values with median
Embarked	Filled missing values with mode
Cabin	Dropped (too many missing values)

Feature Encoding

Converted non-numeric features into numerical form:

Sex → Label Encoding (male = 0, female = 1)

Embarked → One-Hot Encoding (Embarked_Q, Embarked_S)

Feature Scaling

Scaled numerical columns using:

StandardScaler()


Columns scaled:

Age

SibSp

Parch

Encoded columns

(Target Fare not scaled)

Model Training

Modified dataset to use selected features

Split into 80% training and 20% testing

Fitted model using:

LinearRegression()

Model Evaluation

Evaluated the model using regression metrics:

MAE – Mean Absolute Error

MSE – Mean Squared Error

RMSE – Root Mean Squared Error

R² Score – Goodness of Fit

Visualization

Generated multiple ML visualizations:

Actual vs Predicted Fare scatter plot

Residual error distribution plot

Correlation heatmap (optional)

Output

Saved cleaned dataset as:
✔ titanic_cleaned.csv

Training & evaluation logs printed

Plots displayed in the notebook

Tools Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

