# Predictive-Modeling-of-Earthquake-Magnitude-using-Seismic-Data

## Project Overview

* This project implements an end-to-end machine learning pipeline to predict earthquake magnitude using historical seismic data. The system processes structured earthquake-related features, trains a supervised learning model, and deploys the final model as an interactive web application on Streamlit Cloud for real-time prediction.

* The project demonstrates the complete ML lifecycle, including preprocessing, pipeline versioning, model training, evaluation, and production deployment.

## Problem Statement

* Earthquakes pose significant risks to life and infrastructure. While earthquakes cannot be prevented, predictive modeling using historical seismic data can help estimate earthquake magnitude and support preparedness, monitoring, and analytical decision-making.

* The objective of this project is to:

* Analyze seismic attributes associated with earthquakes

* Build a machine learning model to predict earthquake magnitude

* Provide a user-friendly interface for real-time prediction

## Key Challenges

* Seismic data contains noise and variability

* Multiple numerical features influence earthquake magnitude

* Selecting a model that balances interpretability and performance

* Ensuring consistent preprocessing during training and inference

* Deploying a reproducible model for real-time use

## Project Objectives

* Clean and preprocess earthquake-related data

* Engineer meaningful features from seismic parameters

* Train and evaluate machine learning models

* Select the best-performing model

* Deploy the trained pipeline using Streamlit Cloud

## Dataset Description

* Data Type: Structured seismic dataset

## Input Features:

* Latitude

* Longitude

* Depth

* RMS

* Distance metrics

* Error-related seismic parameters

* Target Variable: Earthquake Magnitude

* Source: Publicly available earthquake/seismic datasets

## System Workflow
Raw Seismic Data
   ↓
Data Cleaning & Preprocessing
   ↓
Feature Engineering
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Pipeline Serialization
   ↓
Streamlit Deployment

## Data Preprocessing & Feature Engineering

* The preprocessing pipeline ensures consistency and reproducibility:

* Handling missing and invalid values

* Feature scaling and normalization (where applicable)

* Selection of relevant seismic attributes

* Pipeline versioning to ensure training–inference parity

* All preprocessing steps are embedded within the ML pipeline.

## Model Development
### Selected Model

* Algorithm: Decision Tree Regressor

* Learning Type: Supervised Machine Learning (Regression)

### Why Decision Tree?

* Handles non-linear relationships effectively

* Requires minimal feature scaling

* Easy to interpret decision logic

* Fast inference suitable for deployment

## Model Evaluation

* The model was evaluated using standard regression metrics:

* Mean Absolute Error (MAE)

* Mean Squared Error (MSE)

* Root Mean Squared Error (RMSE)

* These metrics provide insight into the accuracy and reliability of magnitude predictions.

## Deployment – Streamlit Cloud
* Application Overview

* The trained pipeline is deployed as an interactive Streamlit web application, allowing users to:

* Input seismic parameters

* Generate real-time earthquake magnitude predictions

* Interact with the model without local setup

* Deployment Features

* Serialized pipeline (.pkl)

* Real-time inference

* User-friendly UI

* Cloud-hosted accessibility

## Repository Structure
├── version_change_EARTH_QUAKE_PIPELINE_MODEL.ipynb
├── eq_dt_pipeline_2.pkl
├── app.py
├── requirements.txt
├── README.md

## Technology Stack

* Programming Language: Python

* Data Analysis: Pandas, NumPy

* Machine Learning: Scikit-learn (Decision Tree)

* Model Serialization: Pickle

* Deployment: Streamlit Cloud

## Key Outcomes

* Built a complete earthquake magnitude prediction pipeline

* Successfully deployed a real-time prediction application

* Demonstrated ML pipeline versioning and reproducibility

* Applied machine learning to real-world seismic data

## Future Enhancements

* Experiment with ensemble models (Random Forest, Gradient Boosting)

* Incorporate temporal and geospatial features

* Improve performance using hyperparameter tuning

* Add uncertainty estimation to predictions

* Integrate API-based access for broader usage

## Project Links
* Streamlit Cloud Live Demo (optional): **https://earthquake-magnitude-prediction-eq-ml-project-ctbtbggbvuw5z8sv.streamlit.app/**

## Disclaimer

* This project is intended for educational and analytical purposes only and should not be used as a definitive earthquake prediction or warning system.

# Author

* Bathula Venu Gopal
* Data Science Intern @ Innomatics Research Labs
* Former Amazon ML Data Associate
* Focus Areas: Machine Learning, Data Analytics & Model Deployment


