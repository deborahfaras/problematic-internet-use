# Problematic Internet Use Classification

This repository contains the code for a classification model to detect **Problematic Internet Use (PIU)**, developed for the **Child Mind Institute** competition. The model utilizes IMU data and various preprocessing techniques to classify individuals based on their internet usage patterns.

The **`child-mind-institute-competition.ipynb`** notebook consists of **two parts**:

1. **Classifying without Actigraphy Data:** This part of the notebook focuses on classifying PIU using alternative data sources, excluding actigraphy data.
2. **Classifying with Actigraphy Data:** This part of the notebook demonstrates how to use actigraphy data (e.g., accelerometer and gyroscope signals) to classify PIU.

## Features

- **Data Preprocessing:** 
  - Handles missing data with imputation.
  - Normalizes IMU features using MinMaxScaler.
  - Extracts actigraphy features (e.g., accelerometer, gyroscope) for input into the model.

- **Model Architecture:**
  - Encoder-decoder structure with attention layers for effective sequential data processing.
  - Dense layers for classification, with regularization to prevent overfitting.
  - Flexible to handle varying input data shapes.

## Requirements

- Python 3.7+
- TensorFlow (for model training and evaluation)
- Pandas, NumPy (for data manipulation)
- Scikit-learn (for preprocessing)
