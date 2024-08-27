Mushroom Classification Project
Project Description
This project involves developing a machine learning model to classify mushrooms as edible or poisonous based on various features. The code covers data loading, preprocessing, model training, and result submission.

Objective
The goal of this project is to create an accurate classification model using mushroom feature data. The model is trained using the XGBoost library and evaluated with various performance metrics.

Usage Instructions
Prerequisites
To run this project, you need to have the following installed:

Python 3.x
pandas
scikit-learn
xgboost
joblib
google-colab
You can install the required libraries using:

bash
Αντιγραφή κώδικα
pip install pandas scikit-learn xgboost joblib
Data Management
Loading Data: The code loads data from CSV files stored in Google Drive. The load_data() function handles errors such as file not found or empty data.

Data Preprocessing:

Checks if the 'id' column exists in the test data.
Removes the 'id' column and adds necessary columns if they are missing, with default values (e.g., 0).
Modeling
Model Training:

Uses XGBClassifier within a Pipeline that includes data preprocessing (scaling, converting categorical data to numerical values) and model training.
Parameters include eval_metric='mlogloss' and random_state=42.
Model Evaluation:

The model is evaluated using the following metrics:
Accuracy: The proportion of correct predictions.
ROC AUC: The ability of the model to separate classes.
Matthews Correlation Coefficient (MCC): A measure of the model's overall quality, especially on imbalanced datasets.
File Management
Saving and Loading the Model:

The trained model is saved using joblib. The model is loaded from Google Drive and used for predictions.
Creating the Submission File:

Generates a CSV file with the model’s predictions and saves it to Google Drive.
Test Data Processing
The preprocess_test_data() function prepares the test data to match the features expected by the trained model:

Checks if the 'id' column exists and removes it.
Adds missing columns with default values.
Reorders columns to match the model’s expected order.
Exceptions and Errors
The code handles errors during data loading, model training, and submission file creation:

Model Loading Errors:

Verifies if the model is loaded correctly and contains the XGBClassifier.
Data Processing Errors:

Ensures that all necessary data is available and in the correct format.
Contributions
To contribute to the project, fork the repository, make your changes, and submit a pull request.

Contact
For any questions or suggestions, you can contact the author through the provided contact information on their GitHub profile.
