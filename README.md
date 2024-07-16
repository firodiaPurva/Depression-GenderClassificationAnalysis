# Depression and Gender Classification

## Introduction

The Depression and Gender Classification project aims to classify individuals based on their depression levels and gender using machine learning techniques. By leveraging advanced data preprocessing, feature engineering, and various classification algorithms, this analysis provides insights into identifying depression and gender from acoustic features.

## Dataset

The dataset used in this analysis consists of acoustic features extracted from speech recordings. The data includes multiple CSV files for training and testing, with features representing various aspects of speech and corresponding labels for depression and gender.

## Project Objectives

1. **Classify Depression Levels**: Develop a model to accurately classify individuals' depression levels based on acoustic features.
2. **Classify Gender**: Develop a model to classify individuals' gender based on the same set of features.
3. **Evaluate Model Performance**: Assess the performance of various machine learning models in terms of accuracy and fairness across different gender groups.

## Methods

### Data Preprocessing

1. **Data Merging**: Combined multiple CSV files to create a comprehensive dataset for training and testing.
2. **Handling Missing Values**: Implemented strategies to manage any missing values in the dataset.
3. **Feature Scaling**: Normalized and scaled features to ensure they are on a similar scale, improving model performance.
4. **Data Splitting**: Separated the features from the target variables (depression and gender labels) in both training and test datasets.

### Analysis Techniques

1. **Machine Learning Models**: 
   - **Logistic Regression**
   - **Random Forest**
   - **Support Vector Machine**
   - **AdaBoost**
   - **XGBoost**
   - **LightGBM**
   - **Naive Bayes**
2. **Model Evaluation**: 
   - Calculated classification accuracy and balanced accuracy.
   - Assessed True Positive Rate (TPR) for female and male participants.
   - Computed equality of opportunity to evaluate fairness.

### Evaluation Metrics

1. **Accuracy**: Overall correctness of the model.
2. **Balanced Accuracy**: Average of recall obtained on each class.
3. **True Positive Rate (TPR)**: Proportion of actual positives correctly identified.
4. **Equality of Opportunity**: Fairness metric ensuring equal TPR across different groups.

## Results

- **Depression Classification**:
  - Best performance achieved with XGBoost, showing high accuracy and balanced TPR across genders.
  - Logistic Regression and SVM also performed well but showed slight gender bias.
- **Gender Classification**:
  - Random Forest and LightGBM provided good accuracy but varied in TPR for different genders.
  - XGBoost again showed reasonable TPR and equality of opportunity, making it the preferred choice.

## Conclusions

- The analysis successfully classified depression levels and gender based on acoustic features with reasonable accuracy.
- XGBoost emerged as a robust model for both tasks, providing a good balance between accuracy and fairness.
- There is potential to improve model fairness further, ensuring equal performance across gender groups.

## Future Research

1. **Model Enhancement**: Exploring other algorithms and hyperparameter tuning to improve prediction accuracy and fairness.
2. **Extended Features**: Including additional features such as speech content, demographic information, and external factors.
3. **Real-Time Classification**: Implementing real-time classification systems for dynamic and adaptive analysis.
4. **Cross-Domain Analysis**: Analyzing speech patterns across different domains and settings for a more comprehensive understanding.
