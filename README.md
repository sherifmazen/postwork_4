# Predictive Maintenance Analysis - AI4I 2020 Dataset

## Project Overview

This project analyzes the AI4I 2020 Predictive Maintenance Dataset to identify patterns and build machine learning models for predicting machine failures. The analysis includes comprehensive data exploration, visualization, feature engineering, and predictive modeling to support maintenance decision-making.

## Dataset Description

The AI4I 2020 dataset contains operational data from industrial machines with the following features:

- **UDI**: Unique identifier for each record
- **Product ID**: Product identification code
- **Type**: Machine type (L, M, H)
- **Air temperature [K]**: Ambient air temperature in Kelvin
- **Process temperature [K]**: Process temperature in Kelvin
- **Rotational speed [rpm]**: Rotational speed in revolutions per minute
- **Torque [Nm]**: Torque in Newton meters
- **Tool wear [min]**: Tool wear time in minutes
- **Machine failure**: Binary target variable (1 = failure, 0 = no failure)
- **Failure types**: 
  - TWF: Tool Wear Failure
  - HDF: Heat Dissipation Failure
  - PWF: Power Failure
  - OSF: Overstrain Failure
  - RNF: Random Failures

## Project Structure
predictive-maintenance-analysis/
│
├── ai4i2020_analysis.ipynb # Main analysis notebook
├── ai4i2020_processed.csv # Processed dataset (output)
├── requirements.txt # Python dependencies
└── README.md # Project documentation

text

## Key Features

### 1. Data Exploration & Visualization
- Statistical summary and data quality assessment
- Distribution analysis of all variables
- Correlation matrix and heatmap visualization
- Failure pattern analysis by machine type

### 2. Machine Learning Models
- **Logistic Regression**: Baseline classification model
- **Random Forest**: Ensemble method with feature importance
- **Support Vector Machine (SVM)**: Advanced classification

### 3. Model Evaluation
- Accuracy metrics and cross-validation
- Confusion matrix analysis
- Feature importance ranking
- Performance comparison

### 4. Predictive Insights
- Failure rate analysis by operational parameters
- Tool wear and temperature impact assessment
- Maintenance recommendation insights

## Installation & Setup

### Prerequisites
- Python 3.7+
- Google Colab or Jupyter Notebook

### Required Libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly
Usage
Running in Google Colab
Upload the ai4i2020.csv file to Colab

Run the notebook cells sequentially

Download the processed dataset for further analysis

Key Steps
Data Loading: Import and validate dataset

Exploratory Analysis: Understand data distributions and relationships

Preprocessing: Feature encoding and scaling

Model Training: Train multiple classification models

Evaluation: Compare model performance

Insights: Extract maintenance recommendations

Results
Model Performance
The analysis compares three machine learning models:

Logistic Regression: Baseline performance

Random Forest: Typically shows best performance with feature importance

SVM: Alternative approach for complex patterns

Key Findings
Identification of critical failure indicators

Feature importance ranking for maintenance prioritization

Optimal operational parameter ranges

Failure prediction accuracy metrics

Output Files
ai4i2020_processed.csv: Cleaned and feature-engineered dataset

Model performance metrics: Accuracy, precision, recall scores

Visualizations: Distribution plots, correlation matrices, feature importance charts
