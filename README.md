# Dementia-Risk-Prediction-ML-Project-
Spring 2024 - Florida Atlantic University AI in Biology Project 

## Overview

This project focused on building and evaluating supervised machine learning models to predict dementia risk using clinical health data. The dataset was obtained from Kaggle and contained approximately 1,000 patient records with 24 different health-related features, including both continuous and categorical variables.

The goal of this project was not only to create a predictive model, but also to better understand how preprocessing, feature selection, and model evaluation impact machine learning performance in healthcare datasets.

---

## Objectives

* Clean and preprocess clinical health data
* Train and compare multiple supervised learning models
* Reduce overfitting through feature selection
* Evaluate model performance using multiple metrics
* Visualize model behavior and feature importance

---

## Dataset

**Source:** Kaggle – Dementia Patient Health and Prescriptions Dataset

The dataset included:

* ~1,000 patient samples
* 24 clinical and demographic features
* Both continuous and categorical variables
* Missing values and highly correlated features

Some example features included:

* Age
* MRI Delay
* APOE ε4 status
* Depression Status
* Smoking Status
* Blood Oxygen Level
* Cognitive Test Scores

---

## Data Preprocessing

One of the first challenges I came across during this project was determining how to properly preprocess the categorical data. I initially attempted one-hot encoding, but after multiple unsuccessful attempts and further research, I decided to use label encoding instead.

The preprocessing steps included:

* Handling missing values
* Converting categorical variables into numerical values using label encoding
* Splitting the data into training and testing datasets (70/30 split)
* Creating correlation heatmaps to identify highly correlated features
* Removing features that appeared to contribute to overfitting

The three features removed were:

* Prescription
* Dosage in mg
* Cognitive Test Scores

---

## Models Used

The following supervised learning models were trained and evaluated:

* Decision Tree Classifier
* Random Forest Classifier
* Logistic Regression
* Support Vector Machine (SVM)

### Libraries & Tools

* Python
* pandas
* NumPy
* scikit-learn
* matplotlib
* seaborn
* Google Colab

---

## Results

### Random Forest Classifier

* Accuracy: 77%
* AUC: 0.86
* Precision: 0.85
* Recall: 0.65
* F1 Score: 0.73

The Random Forest model performed the best overall and demonstrated strong performance in distinguishing dementia from non-dementia cases while maintaining a balance between sensitivity and specificity.

### Logistic Regression

* Accuracy: 75%
* AUC: 0.84

### Decision Tree

* Accuracy: 68%
* AUC: 0.68

### Support Vector Machine

* Accuracy: 72%

---

## ROC Curve

The ROC curve for the Random Forest model achieved an Area Under the Curve (AUC) of 0.86, demonstrating strong model performance in distinguishing dementia from non-dementia cases.

---

## Precision-Recall Curve

The Precision-Recall curve demonstrated the tradeoff between precision and recall across different classification thresholds. The model maintained relatively strong precision while recall increased, indicating solid predictive capability for identifying dementia cases.

---

## Feature Importance

One interesting observation from the Random Forest model was that the feature “Depression Status” showed the highest feature importance. APOE ε4 status also demonstrated relatively high correlation with dementia.

This project helped me better understand:

* Feature importance analysis
* Overfitting in machine learning models
* Differences between Decision Trees and Random Forests
* The importance of preprocessing and feature selection in healthcare datasets

---

## What I Learned

This project was one of my first deeper experiences with machine learning and healthcare data analysis. During this project I learned:

* How to preprocess real-world datasets
* How to evaluate model performance using ROC curves, AUC, precision, recall, and F1-score
* How Random Forest models reduce overfitting compared to individual Decision Trees
* The importance of reproducibility and proper train-test splitting
* How visualization tools can help interpret machine learning results

I also learned that building a model is only one part of the process. Understanding why a model performs a certain way and identifying possible sources of bias or overfitting are equally important.

---

## Future Improvements

If I continued this project, I would:

* Further investigate potential feature bias from Depression Status and APOE ε4
* Experiment with additional preprocessing methods
* Tune hyperparameters to improve performance
* Explore cross-validation techniques
* Test additional machine learning models

---

## Files Included

* Dementia ML Project Proposal
* Final Project Presentation
* Google Colab Notebook / Code
* Model evaluation plots and visualizations

---

## Author

Guevna “Nina” Prosper
MS Bioinformatics Student – Northeastern University
