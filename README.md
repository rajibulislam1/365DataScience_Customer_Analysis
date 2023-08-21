# Black-Friday-free-offer-plan-purchasing-a-subscription
The likelihood of a student registered for a free plan purchasing a subscription on the 365datascience.com online teaching platform.
The decision is based on students’ activities on the platform—viewing lectures and participating in exams.
The project is inspired by an initiative 365 had in 2022 to predict student purchases before our Black Friday campaign. We wanted to create a list of students likelier to purchase and retarget them with unique ads on social media. But as it turned out, this was no easy task due to the extreme imbalance of the data—the number of students who had never purchased a subscription was much higher than the number of students who had. The primary reason for that was the free campaign we ran before the Black Friday one, where the platform was unlocked for free to all 365 students.

As you will see, such class imbalance combined with humans’ unpredictable behavior makes it challenging to predict student purchases.

# I have completed the project with five different Algorithms accordingly
 *Logistic Regression 
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













