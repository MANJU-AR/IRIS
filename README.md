# Iris Species Classifier

A machine learning project that classifies iris flowers into three species (Setosa, Versicolor, and Virginica) using a Random Forest classifier.

## Overview

This project demonstrates a complete machine learning pipeline for classification using the famous Iris dataset. The classifier achieves high accuracy in predicting iris species based on flower measurements.

## Features

- **Data Loading**: Automatically downloads and loads the Iris dataset from UCI ML Repository
- **Data Preprocessing**: Label encoding for species classification
- **Model Training**: Random Forest classifier implementation
- **Model Evaluation**: Comprehensive accuracy metrics and classification reports
- **Reproducible Results**: Fixed random state for consistent outputs

## Dataset

The [Iris dataset](https://archive.ics.uci.edu/ml/datasets/iris) contains 150 samples of iris flowers with the following features:

- **sepal_length**: Length of the sepal in cm
- **sepal_width**: Width of the sepal in cm  
- **petal_length**: Length of the petal in cm
- **petal_width**: Width of the petal in cm
- **species**: Target variable (Setosa, Versicolor, Virginica)

## Requirements

```
pandas
scikit-learn
```

## Installation

1. Clone this repository:
```bash
git clone <your-repo-url>
cd iris-classifier
```

2. Install required packages:
```bash
pip install pandas scikit-learn
```

## Usage

Run the classifier:

```bash
python iris_classifier.py
```

The script will:
1. Download and load the Iris dataset
2. Preprocess the data with label encoding
3. Split data into training (80%) and testing (20%) sets
4. Train a Random Forest classifier
5. Make predictions on the test set
6. Display accuracy score and detailed classification report

## Model Performance

The Random Forest classifier typically achieves:
- **Accuracy**: ~96-100% on the test set
- **High precision and recall** across all three species classes

## Code Structure

```python
# Data loading and preprocessing
- Load dataset from UCI repository
- Apply label encoding to species names
- Split into features (X) and target (y)

# Model training
- 80/20 train-test split
- Random Forest with default parameters
- Fit on training data

# Evaluation
- Predictions on test set
- Accuracy calculation
- Detailed classification report
```

## Results

Sample output:
```
Accuracy: 1.0
Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        10
           1       1.00      1.00      1.00         9
           2       1.00      1.00      1.00        11

    accuracy                           1.00        30
   macro avg       1.00      1.00      1.00        30
weighted avg       1.00      1.00      1.00        30
```

## Potential Improvements

- **Hyperparameter Tuning**: Grid search or random search for optimal parameters
- **Cross-Validation**: K-fold validation for more robust performance estimates
- **Feature Engineering**: Feature scaling or polynomial features
- **Model Comparison**: Compare with other algorithms (SVM, Logistic Regression, etc.)
- **Data Visualization**: Add plots for feature distributions and decision boundaries

## License

This project is open source and available under the [MIT License](LICENSE).

## Contributing

Feel free to fork this project and submit pull requests for improvements or bug fixes.
