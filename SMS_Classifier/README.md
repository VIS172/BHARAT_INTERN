![1_-IwVhfTvy_PKe_cmpmBTKg](https://github.com/VIS172/BHARAT_INTERN/assets/109724129/d4e31a25-8dd8-4228-945c-0968a3bc3078)


# SMS Classifier Project

The SMS classifier implemented in Python using machine learning models is designed to distinguish between spam and ham (non-spam) messages.

## Features

- Preprocessing of SMS data
- Feature extraction using TF-IDF vectorization
- Implementation of multiple classifiers (e.g., SVM, MultinomialNB, Extra Trees)
- Evaluation of classifier performance (accuracy and precision)
- Model serialization using pickle
- Ensemble learning with Voting Classifier

## Getting Started

### Prerequisites

- Python 3.x
- Required Python libraries (can be installed via `requirements.txt`)

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/sms-classifier.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd sms-classifier
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the script**:
    ```bash
    python sms_classifier.py
    ```

## Code Overview

### 1. Preprocessing and Feature Extraction

- **Text Preprocessing**: Converting text to lowercase, removing punctuation, and tokenizing.
- **TF-IDF Vectorization**: Transforming the text data into TF-IDF features.
- **Pickle Serialization**: Saving the TF-IDF vectorizer to a file.

### 2. Classifiers

- **Support Vector Classifier (SVC)** with sigmoid kernel
- **Multinomial Naive Bayes (MNB)**
- **Extra Trees Classifier (ETC)**
- **Voting Classifier**: An ensemble model combining SVC, MNB, and ETC.

### 3. Model Training and Evaluation

- **Training**: Fitting the models to the training data.
- **Evaluation**: Calculating accuracy and precision of the models.
- **Pickle Serialization**: Saving the trained models to files.

## Usage

### Train and Evaluate Models

The `sms_classifier.py` script includes code for training multiple classifiers and evaluating their performance. The results are printed out with accuracy and precision scores.

### Serialize Models

Models and vectorizers are serialized using `pickle` for later use:
```python
import pickle

# Save the TF-IDF vectorizer
pickle.dump(tfidf, open('vectorizer.pkl', 'wb'))

# Save the MultinomialNB model
pickle.dump(mnb, open('model.pkl', 'wb'))
