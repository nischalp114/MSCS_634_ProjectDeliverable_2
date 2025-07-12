Deliverable 2: Regression Modeling and Performance Evaluation


GROUP MEMBERS:
Name: Nischal Pokharel

Name: Swarna Anjani Devershetty

Name: Vishnu Mallam

Name: Tejeswar Reddy Chemikala

Name: Shyam Nath

Dataset Summary
For this phase of the project, we continued working with the Stroke Prediction Dataset from Kaggle. The dataset contains 5,110 records and 11 features including demographic and health-related information. Although the original use case is classification (predicting stroke), this deliverable focuses on using regression to predict the average glucose level, a continuous numeric variable.

Key features used in modeling include:

age

gender

bmi

hypertension

heart_disease

smoking_status

work_type

ever_married

Residence_type

Steps Taken
Data Cleaning:

Removed rows with ambiguous values such as “Other” in the gender column.

Handled missing values in the bmi column using median imputation.

Dropped duplicate records.

Data Preprocessing:

One-hot encoded categorical variables to prepare them for modeling.

Standardized all numerical features using StandardScaler.

Regression Modeling:

Built two regression models:

Linear Regression

Ridge Regression

The models were trained to predict avg_glucose_level.

Model Evaluation:

Evaluated both models using:

R² Score

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Compared model performance using a bar chart visualization.

Cross-Validation:

Used 5-fold cross-validation to test how well each model generalizes.

Calculated and reported the average R² score across folds.

Key Insights
Both Linear and Ridge Regression models gave nearly identical results:

R² Score: ~0.0900

MSE: ~0.0519

RMSE: ~0.2277

The low R² values indicate that the models are not strong predictors of glucose level, suggesting that other unmeasured factors may play a larger role.

The consistent cross-validation scores indicate that both models are stable and not overfitting.

Challenges
The dataset was originally designed for classification, not regression, which limited model performance.

Glucose levels are influenced by many lifestyle and medical factors not included in this dataset.

Some categorical variables had many unique values, making encoding and modeling more complex.

Files Included
Deliverable2.ipynb: A Jupyter Notebook containing all data cleaning, preprocessing, modeling, evaluation, and visualizations.

README.md: This file, summarizing the dataset, steps taken, model results, insights gained, and challenges encountered.

