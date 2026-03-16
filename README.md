# Housing Price Regression Models

## Overview

This project demonstrates the implementation and analysis of different regression models used in machine learning. The goal of this project is to understand how various regression techniques work and how they behave when applied to a housing dataset.

The models implemented in this project include:

* Linear Regression
* Ridge Regression
* Lasso Regression

The project also analyzes how regularization affects model performance and feature importance.

---

## Objectives

The main objectives of this project are:

* To understand the concept of regression in machine learning.
* To implement Linear, Ridge, and Lasso regression models.
* To compare model performance using Mean Squared Error (MSE).
* To analyze how the regularization parameter (lambda / alpha) affects Ridge regression.
* To observe how Lasso regression performs feature selection by shrinking coefficients.

---

## Dataset

The project uses a housing dataset containing numerical features related to housing information.

Example features include:

* Median income
* Housing age
* Average number of rooms
* Population
* Average occupancy
* Latitude
* Longitude

Target Variable:

* **Median House Value**

Only numerical features are used for training the regression models.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

---

## Models Implemented

### 1. Linear Regression

Linear Regression is a basic regression model that attempts to model the relationship between input features and the target variable using a straight line.

It minimizes the Mean Squared Error between predicted and actual values.

---

### 2. Ridge Regression

Ridge Regression is a regularized version of Linear Regression that introduces an **L2 penalty** to the loss function.

This helps:

* Reduce overfitting
* Stabilize model coefficients
* Improve generalization

The regularization strength is controlled by the parameter **alpha (λ)**.

---

### 3. Lasso Regression

Lasso Regression introduces an **L1 penalty** to the model.

Key advantages:

* Performs feature selection
* Can shrink some coefficients to exactly zero
* Helps simplify the model

---

## Model Evaluation

The models are evaluated using:

**Mean Squared Error (MSE)**

MSE measures the average squared difference between predicted and actual values.

Lower MSE indicates better model performance.

---

## Ridge Regularization Analysis

The project also studies how different values of **lambda (α)** affect model performance.

The following lambda values were tested:

0.01, 0.1, 1, 10, 100

A graph is generated showing:

* Training Error
* Testing Error

This helps visualize how regularization impacts bias and variance.

---

## Lasso Feature Analysis

Lasso regression coefficients are analyzed to determine whether features are eliminated.

Features with coefficient value **0** are considered removed by the model.

This demonstrates how Lasso can perform automatic feature selection.

---

## Project Structure

housing-regression-ml
│
├── housing.csv
├── regression_models.ipynb
├── ridge_lasso_analysis.ipynb
└── README.md

---

## Results

The project prints:

* Mean Squared Error for each regression model
* Model coefficients
* Number of features eliminated by Lasso
* Graph showing lambda vs error for Ridge regression

---

## Future Work

Future improvements to this project include:

* Implementing a complete **House Price Prediction System**
* Adding **Cross Validation**
* Hyperparameter tuning
* Feature engineering
* Model comparison with advanced algorithms
