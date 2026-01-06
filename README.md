# titanic-data

Project Overview

This project analyzes the famous Titanic dataset to understand which factors influenced passenger survival during the Titanic disaster.
Using data science techniques and machine learning, we explore passenger data, clean and preprocess it, visualize important patterns, and build predictive models to estimate survival chances.

This project is widely used as a beginner-to-intermediate level classification problem and demonstrates a complete end-to-end data science workflow.

Dataset Description

The dataset contains information about passengers who were aboard the Titanic, including demographic details, ticket information, and survival status.

Target Variable

Survived

0 → Passenger did not survive

1 → Passenger survived

This is a binary classification problem.

🧾 Feature Description

Each row represents a single passenger with the following attributes:

Feature	Description
PassengerId	Unique passenger identifier
Survived	Survival status (Target variable)
Pclass	Passenger class (1 = Upper, 2 = Middle, 3 = Lower)
Name	Passenger name
Sex	Gender of the passenger
Age	Age in years
SibSp	Number of siblings/spouses aboard
Parch	Number of parents/children aboard
Ticket	Ticket number


What This Dataset Tells Us

The dataset helps us understand social and economic factors that affected survival chances:

Women had a higher survival rate than men

Passengers in higher classes survived more

Children had better survival chances

Fare and class were strong indicators of survival

Survival was not random; it followed clear patterns

This makes the dataset ideal for classification modeling and exploratory analysis.

Step-by-Step Explanation of the Notebook
(1) Importing Required Libraries

All necessary Python libraries are imported to support data handling, visualization, and machine learning.

(2) Loading the Dataset

The dataset is loaded using Pandas, allowing structured access to rows and columns.
Initial inspection helps identify:

Dataset size

Column names

Data types

(3) Exploratory Data Analysis (EDA)

EDA is performed to understand patterns and trends:

Checking missing values

Analyzing survival distribution

Comparing survival rates by gender, class, and age

Understanding fare distribution

EDA helps answer real-world questions such as “Who was more likely to survive?”

(4) Data Cleaning

Real-world datasets contain missing and inconsistent data. In this step:

Missing Age values are handled

Missing Embarked values are filled

Irrelevant features like Name, Ticket, and Cabin are removed

Categorical data is prepared for encoding

(5) Feature Engineering

To make the dataset suitable for machine learning:

Sex is converted into numerical format

Embarked is encoded

Selected relevant features are retained

Dataset is converted into a numeric matrix

This step ensures better model performance.

(6) Splitting the Dataset

The data is split into:

Training set → Used to train the model

Testing set → Used to evaluate predictions

This prevents overfitting and improves generalization.

(7) Model Building

A classification algorithm is applied to predict survival:

The model learns patterns from passenger data

It predicts whether a passenger survived or not

Classification is used because the output is binary (0 or 1).

(8) Model Evaluation

The model is evaluated using metrics such as:

Accuracy Score

Confusion Matrix

Classification Report

These metrics help measure how well the model performs.
