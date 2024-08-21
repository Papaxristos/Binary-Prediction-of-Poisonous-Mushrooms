Mushroom Classification: Kaggle Playground Series 2024
Welcome to my submission for the 2024 Kaggle Playground Series competition! The goal of this challenge is to predict whether a mushroom is edible or poisonous based on its physical characteristics.

Overview
This repository contains the code and models used to predict the edibility of mushrooms. The project involves loading data, preprocessing, training a model, and generating predictions. The evaluation metric for this competition is the Matthews Correlation Coefficient (MCC).

Competition Details
Start Date: August 1, 2024
Final Submission Deadline: August 31, 2024
Evaluation Metric: Matthews Correlation Coefficient (MCC)
The objective is to predict whether mushrooms are edible (e) or poisonous (p) based on their physical features.

Files
train.csv: Training data containing mushroom features and their labels.
test.csv: Test data with mushroom features for which predictions are required.
submission.csv: The file to submit containing the predictions for the test data.
Directory Structure
bash
Αντιγραφή κώδικα
/content/drive/MyDrive/Python Projects/Mushrooms
│
├── train.csv
├── test.csv
├── submission.csv
└── trained_model.joblib
Workflow
Google Drive Integration: Connects to Google Drive to load and save files.
Data Loading and Exploration: Loads the training and test datasets, checks for missing values, and displays basic information about the data.
Data Preprocessing: Identifies categorical and numerical features, then applies preprocessing steps including imputation and scaling.
Model Training: Uses a Logistic Regression model trained on the processed training data.
Model Evaluation: Calculates training accuracy.
Test Data Processing: Prepares test data for predictions by aligning columns with the trained model.
Prediction and Submission: Generates predictions on the test data and saves them in a submission file.
Requirements
Python 3.x
pandas
numpy
scikit-learn
joblib
google-colab
Installation
To run the code, ensure you have the required libraries installed. You can install them using pip:

bash
pip install pandas numpy scikit-learn joblib
Usage
Mount Google Drive: The script mounts Google Drive to access datasets.
Run the Script: Execute the code to load data, train the model, and generate predictions.
Results
The trained model is saved as trained_model.joblib in Google Drive. Predictions are saved in submission.csv.

Citation
Reade, W., & Chow, A. (2024). Binary Prediction of Poisonous Mushrooms. Kaggle. Kaggle Competition

License
This project is licensed under the MIT License - see the LICENSE file for details.
