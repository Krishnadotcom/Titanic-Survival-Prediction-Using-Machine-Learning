# Machine-Learning-Model-for-Predictive-Data-Analysis
Developed as part of an academic group project, this repository demonstrates a full machine learning pipeline — from data preprocessing and visualization to model training and evaluation. The dataset, sourced from Kaggle, is analyzed and modeled using Python and key ML libraries such as scikit-learn, pandas, and matplotlib. This project aims to build and evaluate machine learning models to predict the survival of passengers on the Titanic using the provided dataset. The process involves several key stages: data loading and initial analysis, data preprocessing to handle missing values and prepare features, data visualization to understand relationships within the data, and finally, training and evaluating different machine learning models to predict survival.

### Project Workflow Summary

#### **Step 1: Importing Libraries and Loading Data**
- Imported essential Python libraries:
  - `pandas` for data manipulation
  - `matplotlib` and `seaborn` for visualization
  - `scikit-learn` for machine learning
- Loaded the Titanic passenger dataset into a pandas DataFrame.

#### **Step 2: Data Analysis**
- Performed initial exploration of the dataset:
  - Displayed the first few rows
  - Checked dataset shape (rows and columns)
  - Reviewed data types and non-null values
  - Identified missing values in each column

#### **Step 3: Data Preprocessing**
- Handled missing values:
  - Dropped the `Cabin` column due to excessive missing data
  - Filled missing `Age` values with the mean
  - Filled missing `Embarked` values with the mode (most common value)
- Feature Engineering:
  - Created a new `Family` column by adding `SibSp` and `Parch`
  - Dropped the original `SibSp` and `Parch` columns
- Encoded categorical features (`Sex` and `Embarked`) into numerical form for model compatibility

#### **Step 4: Data Visualization**
- Created visualizations to analyze relationships with survival outcome:
  - Count of survivors vs. non-survivors
  - Survival comparison by gender
  - Survival comparison by passenger class (`Pclass`)
  - Relationship between family size and survival

#### **Step 5: Model Training and Evaluation**
- Split the data into training and testing sets
- Trained three classification models:
  - Logistic Regression
  - Random Forest Classifier
  - Support Vector Machine (SVM)
- Evaluated accuracy on training and testing data
- Compared model performance to determine the best-performing algorithm

#### **Step 6: Testing with New Data**
- Loaded a separate test dataset and actual survival results (`gender_submission.csv`)
- Applied the same preprocessing steps to the test data
- Generated predictions using each trained model
- Compared predictions to actual outcomes to calculate final accuracy scores
- Assessed model performance on unseen data

---

This project demonstrates a complete machine learning classification workflow — from data exploration and preprocessing to model training, evaluation, and final testing.
