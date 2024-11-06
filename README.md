
# Customer Churn Prediction for a Telecom Company

This project uses machine learning to predict customer churn in a telecom company, allowing the company to identify customers who may be likely to leave. Using Random Forest and advanced feature engineering, we aim to improve prediction accuracy by capturing complex patterns in customer data.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Features](#features)
- [Modeling](#modeling)
- [Results](#results)
- [Usage](#usage)
- [License](#license)

## Project Overview
Customer churn prediction is essential for improving customer retention, especially in subscription-based industries. By analyzing various features, including service usage and billing information, this model predicts churn risk, enabling proactive business strategies.

## Dataset
The dataset includes key customer information, such as:
- `MonthlyCharges`: Monthly charges for the customer's subscription
- `TotalCharges`: Accumulated charges for the customer's account
- `tenure`: Duration (in months) the customer has been with the company
- `Churn`: Whether the customer has left or stayed with the company (target variable)

**Data Source:** [Telecom_Customer_Churn.csv](./Telecom_Customer_Churn.csv) 

This dataset contains customer information from a telecom company, including service usage, billing information, and churn status.

## Project Structure
```
Customer-Churn-Prediction-for-a-Telecom-Company-main/
├── Telecom_Customer_Churn.csv      # Dataset file
├── Untitled.ipynb                  # Jupyter notebook for EDA and modeling
├── README.md                       # Project documentation
└── requirements.txt                # Package dependencies
```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/als138/Customer-Churn-Prediction-for-a-Telecom-Company.git
   cd Customer-Churn-Prediction-for-a-Telecom-Company-main
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Features
In addition to the dataset’s original features, new features have been created to improve model performance:
- **Interaction Features**: Generated features from interactions, such as `TotalSpent = MonthlyCharges * tenure`.
- **Polynomial and Log Transformations**: Features transformed to highlight non-linear relationships.
- **PCA Components**: Dimensionality reduction using PCA to control feature complexity.

## Modeling
The project utilizes a **Random Forest Classifier** to capture non-linear relationships in the data. Cross-validation is used to ensure model robustness, and metrics such as accuracy, precision, recall, and F1-score are reported.

#### Confusion Matrix and Performance Report
The model's performance is evaluated through a confusion matrix and detailed classification metrics.

## Results
The model achieves strong performance in predicting customer churn. Key evaluation metrics include:
- **Accuracy:** 79%

## Usage
To run the model and perform data analysis:
1. Open `Untitled.ipynb` in Jupyter Notebook:
   ```bash
   jupyter notebook Untitled.ipynb
   ```
2. Follow the notebook steps to explore the dataset, preprocess data, and train the model.
3. Evaluation metrics and confusion matrix will be generated and displayed.
