# CreditWise: Loan Approval Prediction System

## Project Overview

CreditWise is a machine learning project designed to predict whether a loan application is likely to be approved based on an applicant's demographic, financial, and credit-related information. The system aims to assist financial institutions in making faster and more data-driven lending decisions.

---

## Problem Statement

Manual loan approval processes can be time-consuming and susceptible to inconsistencies. By leveraging historical applicant data and machine learning techniques, this project seeks to automate and improve the loan approval decision-making process.

The objectives of this project are to:

- Analyze factors influencing loan approvals.
- Preprocess and prepare loan application data.
- Build predictive models for loan approval classification.
- Compare multiple machine learning algorithms.
- Identify the best-performing model based on evaluation metrics.

---

## Dataset Features

The dataset includes applicant information such as:

- Applicant Income
- Co-applicant Income
- Credit Score
- Debt-to-Income (DTI) Ratio
- Savings
- Loan Amount
- Age
- Employment Status
- Employer Category
- Education Level
- Marital Status
- Gender
- Property Area
- Loan Purpose
- Loan Approval Status (Target Variable)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

### 1. Data Loading and Exploration

- Imported the loan approval dataset.
- Performed exploratory analysis using:
  - `head()`
  - `info()`
  - `describe()`
  - Missing value inspection.

---

### 2. Missing Value Handling

Applied imputation techniques to handle incomplete data:

- **Numerical Features:** Mean Imputation
- **Categorical Features:** Most Frequent Value Imputation

---

### 3. Exploratory Data Analysis (EDA)

Performed visual analysis to understand the dataset:

- Loan approval distribution.
- Loan purpose frequency analysis.
- Income distribution plots.
- Boxplots comparing financial factors with loan approval.
- Credit score analysis based on approval status.
- Correlation heatmap for numerical features.

---

### 4. Feature Engineering

Created additional features to capture non-linear relationships:

- `DTI_Ratio_sq`
- `Credit_Score_sq`

These engineered features were used to improve model performance.

---

### 5. Feature Encoding

Applied encoding techniques to transform categorical variables:

#### Label Encoding
Used for:

- Education Level
- Loan Approval Status

#### One-Hot Encoding
Used for:

- Employment Status
- Marital Status
- Loan Purpose
- Property Area
- Gender
- Employer Category

---

### 6. Data Preprocessing

- Removed irrelevant identifiers such as Applicant ID.
- Split the dataset into training and testing sets.
- Standardized features using **StandardScaler**.

---

### 7. Model Building

The following classification algorithms were implemented and evaluated:

#### Logistic Regression
A baseline linear classification model for predicting loan approval.

#### K-Nearest Neighbors (KNN)
A distance-based algorithm that classifies applicants using neighboring observations.

#### Gaussian Naive Bayes
A probabilistic classifier that assumes feature independence.

---

### 8. Model Evaluation

Models were evaluated using:

- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- Confusion Matrix

---

## Results

After comparing the performance of all models, **Gaussian Naive Bayes** emerged as the best-performing model based on the selected evaluation criteria, particularly precision.

Feature engineering further enhanced predictive performance.

---

## Business Applications

This system can help financial institutions by:

- Reducing loan processing time.
- Supporting consistent lending decisions.
- Identifying high-risk applicants.
- Improving operational efficiency.
- Assisting loan officers with decision support.

---


