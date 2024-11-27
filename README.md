# Loan Approval Prediction

This repository contains a machine learning project focused on predicting loan approval statuses using historical loan data. The project explores data preprocessing, visualization, and classification techniques to build a predictive model.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Results](#results)
- [Setup](#setup)
- [Usage](#usage)
- [Technologies](#technologies)
- [Acknowledgments](#acknowledgments)

## Overview

Loan approval prediction is critical for financial institutions to assess the risk of approving loans for applicants. This project involves:
- Cleaning and preprocessing loan application data.
- Visualizing key data distributions.
- Building and evaluating a machine learning model for predicting loan approval.

## Features

The project performs:
- Handling missing values in categorical and numerical columns.
- Removing outliers in income and loan-related features.
- Exploratory Data Analysis (EDA) to identify patterns and relationships.
- Building a predictive model using **Support Vector Machine (SVC)**.

## Data Preprocessing

- **Missing Values**: Filled categorical columns with the mode and numerical columns with the median.
- **Outlier Removal**: Applied Interquartile Range (IQR) method for income and co-applicant income.
- **Feature Engineering**: Converted categorical data to numerical using one-hot encoding.
- **Feature Scaling**: Applied `StandardScaler` to numerical features for uniform scaling.

## Modeling

- **Algorithm**: Support Vector Machine (SVC)
- **Train-Test Split**: Data split into 80% training and 20% testing.
- **Evaluation**: The model predicts loan approval status for test data.

## Results

The project demonstrates a streamlined process for loan prediction, enabling financial institutions to make data-driven decisions. Model predictions are added back to the test dataset for evaluation and visualization.

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/username/LoanApprovalPrediction.git
   cd LoanApprovalPrediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset and place it in the project directory:
   ```bash
   loan_prediction.csv
   ```

4. Run the script:
   ```bash
   python loan_approval_prediction.py
   ```

## Usage

- **Visualizations**: The script generates charts using Plotly to explore relationships between variables.
- **Predictions**: Loan approval predictions are stored in the output DataFrame alongside original features.

## Technologies

- **Python**: Core programming language.
- **Libraries**:
  - `pandas`, `numpy` for data manipulation.
  - `scikit-learn` for machine learning.
  - `plotly` for interactive visualizations.

## Acknowledgments

- The dataset and problem statement were inspired by loan prediction challenges in the financial industry.

---

