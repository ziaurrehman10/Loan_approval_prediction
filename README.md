# Loan Approval Prediction Using Artificial Neural Network (ANN)

## Objective

The objective of this project is to build an Artificial Neural Network (ANN) model to predict whether a loan application will be approved based on applicant and loan-related information.

## Dataset

The dataset contains customer demographic, financial, and loan-related attributes along with the target variable **loan_status**.

## Data Preprocessing

The following preprocessing steps were performed:

* Loaded the dataset using Pandas.
* Explored the data using `head()`, `info()`, and `describe()`.
* Checked for missing values and duplicate records.
* Removed the `customer_id` column since it is only an identifier.
* Converted all categorical (`object`) columns into numeric values using `LabelEncoder`.
* Split the dataset into training (80%) and testing (20%) sets.
* Standardized the feature values using `StandardScaler`.

## ANN Architecture

The neural network consists of:

* Input Layer
* Hidden Layer 1: 64 neurons with ReLU activation
* Hidden Layer 2: 32 neurons with ReLU activation
* Hidden Layer 3: 16 neurons with ReLU activation
* Output Layer: 1 neuron with Sigmoid activation

## Model Compilation

* Optimizer: Adam
* Loss Function: Binary Crossentropy
* Evaluation Metric: Accuracy

## Training

The model was trained for 30 epochs with a batch size of 32 while monitoring validation accuracy and validation loss.

## Evaluation

The trained model was evaluated using:

* Test Accuracy
* Test Loss
* Confusion Matrix
* Classification Report

Training and validation accuracy/loss graphs were also generated to analyze the learning process and detect possible overfitting.

## Conclusion

The ANN successfully learned the patterns in the dataset and was able to classify loan approval status effectively. The project demonstrates the complete workflow of building and evaluating a neural network for a binary classification problem.
