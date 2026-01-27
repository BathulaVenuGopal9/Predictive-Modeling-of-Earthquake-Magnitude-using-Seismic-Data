# Predictive Modeling of Earthquake Magnitude Using Seismic Data
## Project Overview

This project implements an end-to-end machine learning pipeline to predict earthquake magnitude using historical seismic data. The system processes structured earthquake-related features, trains an optimized Random Forest Regressor, and deploys the final model as an interactive web application for real-time prediction.

The project demonstrates the complete ML lifecycle including:

Data preprocessing

Pipeline creation and versioning

Model training and hyperparameter tuning

Model evaluation

Production deployment

## Problem Statement

Earthquakes pose significant risks to life and infrastructure. While earthquakes cannot be prevented, predictive modeling using historical seismic data can help estimate earthquake magnitude and support preparedness, monitoring, and analytical decision-making.

The objective of this project is to:

Analyze seismic attributes associated with earthquakes

Build a machine learning model to predict earthquake magnitude

Provide a user-friendly interface for real-time prediction

## Key Challenges

Seismic data contains noise and high variability

Multiple numerical features influence earthquake magnitude

Selecting a model that balances accuracy and generalization

Ensuring consistent preprocessing during training and inference

Deploying a reproducible model for real-time usage

## Project Objectives

Clean and preprocess earthquake-related data

Engineer meaningful features from seismic parameters

Train and evaluate multiple machine learning models

Select the best-performing model using evaluation metrics

Deploy the trained pipeline for real-time prediction

## Dataset Description

Data Type: Structured seismic dataset

Input Features:

Latitude

Longitude

Depth

Dmin

RMS

Horizontal Error

Depth Error

Target Variable:

Earthquake Magnitude

Source:
Publicly available earthquake / seismic datasets

## System Workflow
Raw Seismic Data
      ↓
Data Cleaning & Preprocessing
      ↓
Feature Engineering
      ↓
Model Training & Tuning
      ↓
Model Evaluation
      ↓
Pipeline Serialization
      ↓
Web Application Deployment

## Data Preprocessing & Feature Engineering

The preprocessing pipeline ensures consistency and reproducibility:

Handling missing and invalid values

Feature transformation where required

Selection of relevant seismic attributes

Pipeline versioning to ensure training–inference parity

All preprocessing steps are embedded within the ML pipeline to avoid data leakage and ensure deployment consistency.

## Model Development
### Final Selected Model

Algorithm: Random Forest Regressor
Learning Type: Supervised Machine Learning (Regression)

### Why Random Forest?

Handles non-linear relationships efficiently

Robust against noise and outliers

Reduces overfitting using ensemble averaging

High predictive accuracy

No strict requirement for feature scaling

Suitable for production deployment

### Other Models Evaluated

K-Nearest Neighbors (KNN)

Linear Regression

Decision Tree Regressor

Voting Regressor

Stacking Regressor

AdaBoost Regressor

Gradient Boosting Regressor

XGBoost Regressor

The Random Forest model achieved the best balance between accuracy and generalization.

## Model Evaluation

The models were evaluated using:

R² Score

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Train and test metrics were compared to ensure minimal overfitting and good generalization performance.

## Deployment – Web Application
Application Overview

The trained pipeline is deployed as an interactive web application that allows users to:

Input seismic parameters

Generate real-time earthquake magnitude predictions

Use the model without any local environment setup

Deployment Features

Serialized ML pipeline (.pkl)

Real-time inference

User-friendly interface

Cloud-hosted accessibility

## Repository Structure
├── EARTH_QUAKE_PIPELINE_MODEL.ipynb
├── eq_RANDOMFOREST_pipeline.pkl
├── app.py
├── requirements.txt
├── README.md

## Technology Stack

Programming Language: Python

Data Processing: Pandas, NumPy

Machine Learning: Scikit-learn

Model Serialization: Pickle

Pipeline: Scikit-learn Pipeline + GridSearchCV

Deployment: Gradio / Cloud Hosting

## Key Outcomes

Built a complete earthquake magnitude prediction pipeline

Trained and optimized a Random Forest regression model

Evaluated multiple ensemble algorithms

Successfully deployed a real-time prediction application

Demonstrated ML pipeline versioning and reproducibility

Applied machine learning to real-world seismic data

## Future Enhancements

Experiment with advanced boosting models (LightGBM, CatBoost)

Incorporate temporal and geospatial feature engineering

Improve prediction accuracy with advanced tuning

Add uncertainty estimation to predictions

Provide REST API access for integration

Add live earthquake data integration

## Project Links
* Streamlit Cloud Live Demo (optional): **https://earthquake-magnitude-prediction-eq-ml-project-ctbtbggbvuw5z8sv.streamlit.app/**

## Disclaimer

* This project is intended for educational and analytical purposes only and should not be used as a definitive earthquake prediction or warning system.

# Author

* Bathula Venu Gopal
* Data Science Intern @ Innomatics Research Labs
* Former Amazon ML Data Associate
* Focus Areas: Machine Learning, Data Analytics & Model Deployment


