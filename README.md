**Predicting Median House Values in Boston**

**Objective:**  Utilize multiple linear regression to analyze the relationship between housing characteristics and predict median house values in the Boston area. Focus is placed on the variables 'rm' (average rooms per dwelling) and 'lstat' (percentage of lower status population).

**Data Source:**

Boston Housing Dataset:
Widely used dataset originally published by Harrison and Rubinfeld (1978), obtained from the U.S. Census Service.

**Variables:**

Target Variable:
medv: Median value of owner-occupied homes (in $1000s)
Predictor Variables:
rm: Average number of rooms per dwelling
lstat: Percentage of lower status population
Other Variables (not used in this analysis):
crim, zn, indus, ... (Include a brief description of these as well).
Process:

**Import Libraries:**

pandas: Data manipulation and analysis.
numpy: Numerical calculations.
matplotlib, seaborn: Data visualization.
scikit-learn: Machine learning tools.
Data Loading:

Read the 'boston.csv' file using pd.read_csv().

**Exploratory Analysis:**

Calculate descriptive statistics (df.describe()) to get an overview of the data.
Check for missing values (df.isnull().sum())
Examine correlations between 'rm', 'lstat', and 'medv' using correlation coefficients or visualization (e.g., scatterplots).

**Data Splitting:**

Use train_test_split() to divide the data into:
Training set: To fit the linear regression model
Testing set: To evaluate model performance.

**Model Building:**

Create a linear regression model (LinearRegression()).
Fit the model on the training set with 'rm' and 'lstat' as features.
Evaluation:

Predictions: Generate predictions on the testing set.

**Metrics:**
Mean Squared Error (MSE): Measures average squared prediction error.
R-squared: Explains the proportion of variance in 'medv' explained by the model.

**Interpretation:**

Examine the model's intercept and coefficients.
Interpret how changes in 'rm' and 'lstat' influence the predicted median house value.
Findings:

Summarize the key findings (e.g., signs and magnitudes of the coefficients, MSE, R-squared).
