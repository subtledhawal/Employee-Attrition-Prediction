# Employee Attrition Prediction

This project predicts employee attrition using machine learning techniques. The model is trained to predict whether an employee will leave the company based on various factors like satisfaction level, last evaluation, number of projects, and more. Random Forest Classifier is used as the primary model, and its performance is evaluated using accuracy, precision, recall, and F1-score metrics.

## Table of Contents
- [Project Overview](#project-overview)
- [Data Preprocessing](#data-preprocessing)
- [Data Visualization](#data-visualization)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Cross-Validation](#cross-validation)
- [Installation](#installation)
- [Usage](#usage)

## Project Overview

Employee attrition is a key concern for many organizations. The goal of this project is to predict employee turnover using machine learning models and identify the key factors that contribute to attrition.

## Data Preprocessing

The data is cleaned and preprocessed with the following steps:
- Removing duplicate records.
- Handling missing values.
- Encoding categorical features (`salary`, `Department`) using **Label Encoding**.
- Standardizing numeric features using **StandardScaler**.

## Data Visualization

Data visualizations were created to better understand the distribution and relationships between features. Key visualizations include:
- Bar plots for `salary` and `Department` vs. `left`.
- Box plots for numeric features like `satisfaction_level`, `last_evaluation`, etc.
- Histograms to visualize feature distributions.

## Modeling

- The **Random Forest Classifier** is used for prediction.
- The dataset is split into training and testing sets using an 80-20 split.
- The model is trained on the training set and then evaluated on the test set.

### Hyperparameter Tuning
Grid Search is used to optimize the following hyperparameters:
- `n_estimators`: Number of trees in the forest.
- `max_features`: Number of features considered for splitting.

## Evaluation

The model's performance is evaluated using the following metrics:
- **Confusion Matrix**: Provides insight into true positives, false positives, etc.
- **Accuracy**: Measures overall prediction correctness.
- **Precision**: Measures how many predicted positives are correct.
- **Recall**: Measures how many actual positives were identified.
- **F1-Score**: Harmonic mean of precision and recall.

## Cross-Validation

5-Fold Cross Validation is applied to ensure that the model performs well across different data folds. The average cross-validation accuracy is reported.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/employee-attrition-prediction.git
    cd employee-attrition-prediction
    ```

2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Data Preprocessing**:
   - Load the data and perform cleaning (duplicates, missing values).
   - Encode categorical features and scale numeric features.

2. **Modeling**:
   - Train the Random Forest model on the dataset.
   - Evaluate the model using the test set.

3. **Visualization**:
   - Visualize important features and model performance.

4. **Hyperparameter Tuning**:
   - Use Grid Search to optimize the model parameters.

5. **Cross-Validation**:
   - Perform cross-validation for model validation.
