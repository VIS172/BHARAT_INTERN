![68747470733a2f2f696d61676573382e616c706861636f646572732e636f6d2f3430352f3430353032392e6a7067](https://github.com/VIS172/BHARAT_INTERN/assets/109724129/a6f4f02b-3c7d-4cd0-bc31-dc323b9f4f28)


# Titanic Classification Project

The classifier is designed to predict the likelihood of survival for passengers on the Titanic based on their attributes.

## Features

- Data preprocessing and cleaning
- Feature engineering and selection
- Implementation of multiple classifiers (e.g., Logistic Regression, Decision Trees, Random Forest, SVM, Neural Networks)
- Evaluation of classifier performance (accuracy, precision, recall, F1-score, ROC-AUC)
- Model serialization using pickle
- Ensemble learning with Voting Classifier

## Getting Started

### Prerequisites

- Python 3.x
- Required Python libraries (can be installed via `requirements.txt`)

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/titanic-classification.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd titanic-classification
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Download the dataset**:
    Download the Titanic dataset from [Kaggle](https://www.kaggle.com/c/titanic/data) and place the files in the `data/` directory.

## Code Overview

### 1. Data Preprocessing and Feature Engineering

- **Data Cleaning**: Handling missing values, encoding categorical variables, and normalizing numerical features.
- **Feature Engineering**: Creating new features based on existing ones (e.g., family size, title extraction from names).
- **Pickle Serialization**: Saving the preprocessed data for future use.

### 2. Classifiers

- **Logistic Regression (LR)**
- **Decision Trees (DT)**
- **Random Forest (RF)**
- **Support Vector Machines (SVM)**
- **Neural Networks (NN)**
- **Voting Classifier**: An ensemble model combining LR, DT, and RF.

### 3. Model Training and Evaluation

- **Training**: Fitting the models to the training data.
- **Evaluation**: Calculating accuracy, precision, recall, F1-score, and ROC-AUC for the models.
- **Pickle Serialization**: Saving the trained models to files.

## Usage

### Train and Evaluate Models

The `titanic_classifier.py` script includes code for training multiple classifiers and evaluating their performance. The results are printed out with various evaluation metrics.







