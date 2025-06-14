# Predicting High-Resolution Brain Graphs

This project implements a machine learning approach to predict high-resolution brain graphs from low-resolution input data. The implementation uses Principal Component Analysis (PCA) for dimensionality reduction and Linear Regression for prediction.

## Project Overview

The goal of this project is to develop a method for predicting high-resolution brain connectivity graphs from low-resolution input data. This is particularly useful in scenarios where high-resolution brain imaging data is difficult or expensive to obtain, but low-resolution data is more readily available.

## Methodology

The project implements a two-step approach:

1. **Dimensionality Reduction using PCA**:
   - Reduces the dimensionality of the input features while preserving the most important information
   - Automatically determines the optimal number of components based on the data size
   - Helps in reducing computational complexity and potential overfitting

2. **Linear Regression**:
   - Uses the reduced features to predict high-resolution brain graph values
   - Implements a simple yet effective linear mapping between low and high-resolution data

## Implementation Details

The implementation includes:

- 5-fold cross-validation for robust model evaluation
- Performance metrics:
  - Mean Squared Error (MSE)
  - Mean Absolute Deviation (MAD)
  - Pearson Correlation Coefficient

### Key Functions

- `preprocessing(X_train, X_test, n_components)`: Handles PCA-based feature extraction
- `predict_super_resolution(X_train, Y_train, X_test)`: Implements the prediction pipeline
- `CV_5_Fold(train_LR_location, train_HR_location)`: Performs 5-fold cross-validation
- `write_results(results, file_name)`: Saves prediction results to a file



## Performance

The model's performance is evaluated using:
- Mean Squared Error (MSE)
- Mean Absolute Deviation (MAD)
- Pearson Correlation Coefficient

These metrics provide a comprehensive assessment of the prediction accuracy and reliability.

