# Earthquake Prediction Project

This project aims to develop machine learning models for predicting earthquakes based on historical seismic data. Using various regression and neural network models, the project explores patterns in earthquake occurrences to improve forecasting accuracy, which could enhance early-warning systems for at-risk communities.

## Project Overview

Earthquake prediction is a longstanding challenge due to the complex nature of seismic activity. This project leverages machine learning to analyze relationships between geological features and the likelihood of future earthquakes. By training and comparing several models, including Linear Regression, Support Vector Regression, Random Forest, and Artificial Neural Networks (ANN), we aim to identify patterns that might not be evident through traditional methods.

## Methodology

### 1. Data Preprocessing and Feature Selection

- **Features Used**: Unix time, latitude, longitude, and depth.
- **Reasoning**: Missing values are not replaced by zeros to avoid misinterpretations.
- **Feature Transformation**: Normalization using `MinMaxScaler` ensures each feature contributes equally during training.

### 2. Model Training

The following models were trained to forecast earthquake occurrences:

- **Linear and Polynomial Regression**: Used to establish baseline predictions for seismic activity.
- **Support Vector Regression (SVR)**: Effective in handling outliers and noise, common in seismic datasets.
- **Random Forest Regressor**: Achieved high accuracy and stability in recognizing underlying patterns.
- **Artificial Neural Networks (ANN)**: Captured complex, non-linear patterns, enhancing predictive accuracy.

### 3. Results

Each model's performance was evaluated on the test set, with results as follows:

| Model                | MSE   | R²    |
|----------------------|-------|-------|
| Linear Regression    | 0.008 | 0.445 |
| Polynomial Regression| 0.006 | 0.598 |
| Support Vector Regression | 0.006 | 0.618 |
| Random Forest        | 0.004 | 0.711 |
| Artificial Neural Network | 0.005 | 0.647 |

The **Random Forest** model achieved the highest R² score, indicating strong predictive capabilities in identifying earthquake-related patterns.

## Repository Contents

- **CE784_Project.pdf**: Project report detailing methodologies, models, and results.
- **CE784.ipynb**: Jupyter notebook containing the code and analysis for the project.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/Mids03/model-masters-earthquake-prediction.git
    ```
2. Run ```CE784.ipynb``` to explore data preprocessing, feature extraction, model training, and evaluation steps.

## Contributors
 - **Aashika Gupta**: Linear Regression, ANN Training, Optimization
 - **Mudit Sengar**: Feature Engineering, Random Forest Training
 - **Shambhavi Agarwal**: Data Preprocessing, Polynomial Regression, Model Evaluation
 - **Shrey Patel**: Feature Selection, Support Vector Regression, Report Preparation

 ## References
 1. [Predicting Earthquakes Using Machine Learning](https://medium.com/marionete/predicting-earthquakes-using-machine-learning-21689435dc52)
 2. [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/earthquakes/search/)
 3. [Earthquakes for ML Prediction - Kaggle Dataset](https://www.kaggle.com/datasets/gustavobmgm/earthquakes-for-ml-prediction)

 This project was completed as part of the CE784 course at IIT Kanpur in 2024-25 - I Semester.