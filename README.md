# 365DataScience Customer Analysis for Enhanced Revenue Growth: Leveraging Predictive Insights in Online Marketing
# Introduction:
 The objective of this project was to develop a predictive model to forecast course purchases based on a range of student-related attributes. The dataset encompassed information on variables such as 'minutes_watched', 'courses_started', 'practice_exams_started', 'minutes_spent_on_exams', 'days_on_platform', and 'practice_exams_passed'. The study aimed to ascertain the predictive power of these variables in determining whether a student would make a course purchase.

 I have completed the project with five different Algorithms accordingly
 
 * Logistic Regression 
 * K-Nearest Neighbors
 * Support Vector Machine
 *  Decision Tress algorithm and
 *  Random Forest 


# Data Preprocessing:

* The project started with importing necessary libraries and loading the dataset ('ml_datasource.csv').
* An initial overview of the dataset was obtained using the describe() and dtypes functions.
* The distribution of different variables was visualized using KDE plots to identify potential outliers and skewed data.


# Outlier Removal:

* Outliers were removed from the dataset for several variables, including 'minutes_watched', 'courses_started', 'practice_exams_started', and 'minutes_spent_on_exams'.
* The cleaned dataset without outliers was stored in the variable 'data_no_outliers'.

# Checking for Multicollinearity:

* Variance Inflation Factor (VIF) was calculated to identify multicollinearity among independent variables.
* Variables 'practice_exams_started' and 'practice_exams_passed' were identified as having high VIF > 5 values and were dropped from the dataset.

# Handling NaN Values:

* NaN values in the 'student_country' column were filled with the value 'NAM' to ensure no missing data remained in the dataset.

# Data Splitting:

* The dataset was split into training and testing sets using the train_test_split function from Sklearn.
* The 'purchased' column was separated as the target variable, while the other columns formed the input features.

# Encoding the Data:

* The categorical variable 'student_country' was encoded using the OrdinalEncoder to convert it into a numerical representation.
* The encoder was fit on the training data and applied to both training and test data.

# Creating a Logistic Regression Model:

* The logistic regression model was built using the Logit class from statsmodels.
* Constant terms were added to the scaled training features using add_constant.
* The model was trained on the training data and its summary was printed.
 
# Model Evaluation:

* The trained model was used to predict outcomes on the test set.
* Predicted probabilities were converted to binary predictions (0 or 1).
* The accuracy of the model was calculated by comparing predicted values to actual values.
 
# Additional Model Evaluation:

* The accuracy of the model was evaluated further using the confusion matrix and classification report from sklearn













