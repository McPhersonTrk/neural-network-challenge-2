# neural-network-challenge-2
# Employee Attrition & Department Prediction Model

This project is focused on developing a neural network model to predict employee attrition and department allocation using TensorFlow and scikit-learn. The dataset utilized for training and testing is based on a fictional company's employee attrition data.

## Overview

The model is built using TensorFlow's Keras API and includes preprocessing steps with scikit-learn for handling categorical data and feature scaling. The prediction targets are employee attrition (binary outcome) and department classification (multiclass).

## Dependencies

- pandas
- numpy
- scikit-learn
- TensorFlow

## Dataset

The dataset, `attrition.csv`, is loaded directly from a URL and contains various features related to employee demographics, job characteristics, and performance indicators.

## Features

Selected features for the model include Age, BusinessTravel, DistanceFromHome, Education, and several others. The target variables are `Attrition` and `Department`.

## Preprocessing

Preprocessing steps include:
- Determining unique values for categorical variables
- Encoding categorical features using OneHotEncoder
- Splitting the dataset into training and testing sets
- Scaling features with StandardScaler

## Model Architecture

The neural network consists of an input layer, shared dense layers, and two branches for predicting `Department` and `Attrition`, each ending with their respective output layers. The model uses ReLU activation for hidden layers, softmax for the department prediction, and sigmoid for attrition prediction.

## Compilation and Training

The model is compiled with Adam optimizer and trained using categorical and binary crossentropy losses for department and attrition predictions, respectively. Model accuracy is monitored for both outputs.

## Evaluation

After training, the model is evaluated on a test set, and accuracy for both predictions is reported.

## Usage

To use this project:
1. Ensure all dependencies are installed.
2. Run the provided code in a Python environment.
3. The model will automatically load the dataset, preprocess it, and proceed with training.
4. After training, model performance metrics will be printed.

## Customization

You can customize the selected features, model architecture, and training parameters according to your requirements or to improve model performance.

