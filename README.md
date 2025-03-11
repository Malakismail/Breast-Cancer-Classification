# Breast Cancer Classification with SVM & Logistic Regression

This project demonstrates a complete machine learning workflow on the Breast Cancer dataset from scikit-learn. It includes extensive exploratory data analysis (EDA), data preprocessing, model training using Support Vector Machines (SVM) with various kernels and Logistic Regression, and multiple visualizations to compare model performance.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
  - [SVM Models](#svm-models)
  - [Logistic Regression](#logistic-regression)
- [Evaluation & Visualizations](#evaluation--visualizations)
  - [Classification Reports & Confusion Matrices](#classification-reports--confusion-matrices)
  - [Feature Importance and Correlation Analysis](#feature-importance-and-correlation-analysis)

## Introduction

This repository provides a complete workflow for classifying breast cancer cases using two popular machine learning algorithms: Support Vector Machines (SVM) and Logistic Regression. The project not only covers model training but also emphasizes the importance of Exploratory Data Analysis (EDA) and visualizations in understanding data and model performance.

## Dataset

The dataset used in this project is the Breast Cancer Wisconsin dataset, available in scikit-learn. It includes features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. The target variable indicates whether the tumor is malignant or benign.

## Exploratory Data Analysis (EDA)

Before processing the data, an extensive EDA is performed to:
- Display the first few rows of the dataset
- Check data types and missing values
- Understand the distribution of features with histograms
- Visualize class distribution using countplots
- Explore feature correlations with a heatmap
- Examine pairwise relationships using pairplots

This initial analysis helps in identifying outliers, understanding feature distributions, and detecting multicollinearity.

## Data Preprocessing

Data preprocessing steps include:
- Converting the dataset to a Pandas DataFrame
- Handling missing values (if any)
- Splitting the data into training and testing sets
- Standardizing the features using `StandardScaler` to improve model performance, especially for SVM.

## Modeling

### SVM Models

Multiple SVM models are trained using different kernels:
- **Linear Kernel**
- **Polynomial Kernel**
- **Sigmoid Kernel**
- **Gaussian (RBF) Kernel**

### Logistic Regression

A Logistic Regression model is also trained to provide a baseline comparison against the SVM models.

## Evaluation & Visualizations

The performance of each model is evaluated using:
- **Classification Reports:** Displaying precision, recall, F1-score, and support.
- **Confusion Matrices:** Visualized for all models to show true vs. predicted labels.
- **Precision-Recall Curves:** Useful especially in cases of class imbalance.
- **Feature Importance:** Particularly for Logistic Regression, to understand which features are most influential.
- **Correlation Analysis:** Through a heatmap to identify relationships between features.

An additional function compares training time along with accuracy, precision, recall, and F1-score for all models.


