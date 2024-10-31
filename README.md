# Customer Churn Prediction with ANN

## Project Overview
This project builds an Artificial Neural Network (ANN) to predict customer churn using the Churn_Modelling dataset. By analyzing features related to customer demographics and account details, the model identifies customers likely to leave, enabling data-driven retention strategies.

## Summary

### Data Preparation
- **Loading and Separating Data**: Input features (`X`) and target variable (`Y`) are extracted.
- **Encoding Categorical Features**: Categorical fields (e.g., country, gender) are transformed to numerical values using `LabelEncoder` and `OneHotEncoder`, preparing them for ANN processing.

### Data Splitting and Scaling
- **Data Split**: The dataset is split into 80% training and 20% testing sets.
- **Feature Scaling**: `StandardScaler` standardizes features, enhancing model training and convergence.

### Building the ANN Model
- **Model Initialization**: A `Sequential` model stacks layers for forward processing.
- **Layer Structure**: 
  - Input layer, two hidden layers (with ReLU activation), and an output layer (sigmoid activation for binary output) are added.
  - The output layer’s sigmoid function scales predictions to values between 0 and 1.
- **Compilation**: The model uses the `adam` optimizer and `binary_crossentropy` loss function for binary classification.

### Training and Evaluation
- The model trains over 100 epochs with a batch size of 10.
- Performance is assessed on the test set using a confusion matrix and accuracy score.

## Why This Project
- **Churn Prediction Use Case**: Identifying customers likely to leave is valuable for customer retention strategies.
- **Neural Network Application**: This project showcases how ANNs capture complex patterns for binary classification.
- **Data Preprocessing**: The project demonstrates essential preprocessing steps, including encoding, scaling, and data splitting.

## Requirements
- Python
- NumPy
- Pandas
- Scikit-Learn
- Keras

## Usage
1. Load and preprocess the dataset.
2. Train the model on the training dataset.
3. Evaluate the model on the test dataset for accuracy and performance metrics.

