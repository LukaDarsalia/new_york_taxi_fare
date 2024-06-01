# New York City Taxi Fare Prediction

This project aims to predict taxi fares in New York City using various machine learning models, including linear regression, random forests, XGBoost, and neural networks with transformer-based attention mechanisms. The dataset used is from the [New York City Taxi Fare Prediction](https://www.kaggle.com/competitions/new-york-city-taxi-fare-prediction/overview) competition on Kaggle.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Usage](#usage)
- [Conclusion](#conclusion)

## Introduction
Predicting taxi fares in a busy city like New York requires understanding complex interactions between various factors such as distance, time of day, traffic conditions, and more. This project leverages advanced machine learning techniques to build an accurate fare prediction model.

## Dataset
The dataset consists of millions of taxi rides in New York City, providing details like pickup and dropoff locations, timestamps, passenger counts, and fare amounts.

## Feature Engineering
Key features engineered for the model include:
- **Haversine Distance**: Calculated distance between pickup and dropoff points.
- **Time Features**: Extracted from pickup datetime (hour, day of the week, month).

## Modeling
We experimented with different models, including:
- **Linear Regression**
- **Random Forests**
- **XGBoost**
- **Simple Feed-Forward Neural Network**
- **Attention-based Model (Transformer Encoder)**

## Results
- **XGBoost**: Achieved the best result with an RMSE of 3.17.
- **Random Forests**: Performed well but slightly below XGBoost.
- **Attention-based Neural Network (Transformer Encoder)**: Performed better than linear regression but was not as good as the tree-based models.
- **Linear Regression**: Provided a baseline but was outperformed by other models.

## Usage
To run this project, follow these steps:
1. Clone the repository:
    ```bash
    git clone https://github.com/LukaDarsalia/new_york_taxi_fare.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook:
    ```bash
    jupyter notebook new-york-taxi-fare.ipynb
    ```

## Kaggle Notebook
You can view the full notebook on Kaggle [here](https://www.kaggle.com/code/lukadarsalia/new-york-taxi-fare/notebook).

## Conclusion
This project demonstrates the application of various machine learning models to the task of taxi fare prediction. XGBoost provided the best results, while neural network models with attention mechanisms showed potential for further improvement with more tuning and experimentation. Tree-based models (XGBoost and Random Forests) outperformed linear regression and attention-based models.
