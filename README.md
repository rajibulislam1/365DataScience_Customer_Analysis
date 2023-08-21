# Black-Friday-free-offer-plan-purchasing-a-subscription
The likelihood of a student registered for a free plan purchasing a subscription on the 365datascience.com online teaching platform.
The decision is based on students’ activities on the platform—viewing lectures and participating in exams.
The project is inspired by an initiative 365 had in 2022 to predict student purchases before our Black Friday campaign. We wanted to create a list of students likelier to purchase and retarget them with unique ads on social media. But as it turned out, this was no easy task due to the extreme imbalance of the data—the number of students who had never purchased a subscription was much higher than the number of students who had. The primary reason for that was the free campaign we ran before the Black Friday one, where the platform was unlocked for free to all 365 students.

As you will see, such class imbalance combined with humans’ unpredictable behavior makes it challenging to predict student purchases.


# Data Preprocessing:

* The project started with importing necessary libraries and loading the dataset ('ml_datasource.csv').
* An initial overview of the dataset was obtained using the describe() and dtypes functions.
* The distribution of different variables was visualized using KDE plots to identify potential outliers and skewed data.
