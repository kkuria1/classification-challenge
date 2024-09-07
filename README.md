# Spam Detection Model - README

## Overview

This project is focused on building and evaluating two machine learning models for detecting spam emails based on word frequencies. The dataset used consists of various features representing the frequency of specific words in emails, with the target variable indicating whether the email is spam or not. Two models were trained for this purpose: Logistic Regression and Random Forest Classifier.

## Models Used

1. **Logistic Regression**: A linear model used for binary classification.
2. **Random Forest Classifier**: An ensemble learning method that constructs multiple decision trees to improve classification performance.

## Dataset

The dataset used for this project contains word frequency counts and labels representing whether the email is spam (1) or not spam (0). The dataset has 57 features and a target column (`spam`).

### Data Preparation

- The dataset was split into training (70%) and testing (30%) sets using `train_test_split`.
- Features were standardized using `StandardScaler` to improve model performance, especially for Logistic Regression.

## Project Structure

- **Data Preprocessing**:
    - The data was split into training and testing sets.
    - Features were scaled using `StandardScaler`.
    
- **Model Training**:
    - Two models were trained: Logistic Regression and Random Forest Classifier.
    
- **Model Evaluation**:
    - Both models were evaluated using accuracy on the test set.
    
## Results

- **Logistic Regression Accuracy**: 92.25%
- **Random Forest Accuracy**: 95.66%

### Conclusion

The Random Forest Classifier outperformed Logistic Regression in this project, achieving a higher accuracy of 95.66% compared to 92.25% for Logistic Regression. This result aligns with expectations, as Random Forests are typically better at handling non-linear relationships and feature importance.

## How to Run the Project

1. Clone the repository or download the code files.
2. Install the necessary dependencies by running:
   ```
   pip install -r requirements.txt
   ```
3. Load the dataset or use the provided simulated dataset.
4. Run the Jupyter notebook or Python script to train the models and evaluate their performance.

## Dependencies

- Python 3.x
- scikit-learn
- pandas
- numpy

## Future Work

- **Hyperparameter Tuning**: Improve model performance through grid search or random search for hyperparameter optimization.
- **Feature Engineering**: Explore feature selection and engineering techniques to reduce noise and improve model accuracy.
- **Additional Models**: Test other machine learning models such as Support Vector Machines (SVM) or Neural Networks.

## License

This project is licensed under the MIT License.

---

