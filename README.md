# Network Intrusion Detection
## Overview
This app uses a trained XGBoost model to predict whether network traffic is an attack or benign based on input features.

## Requirements
- Python 3.x
- Gradio
- XGBoost
- Pandas
- NumPy
- Pickle

## Installation
1. Clone the repository or download the code.
2. Install the required libraries using pip: pip install gradio xgboost pandas numpy
3. Load the saved XGBoost model (best_xgb_model.pkl) into the app.

## Usage
1. Launch the app using iface.launch(share=True).
2. Enter network traffic features into the input Dataframe.
3. Click the "Submit" button to generate a prediction.
4. The app will output either "Attack" or "Benign" based on the prediction.

## Input Features
The app expects input features to match the columns of the training data (X_train.columns). The input Dataframe should have the same column names and data types.

## Model
The app uses a trained XGBoost model (best_xgb_model.pkl) to make predictions. The model was trained on a dataset of network traffic features and labels.

## Examples
The app provides a few example inputs in the "Examples" tab. These can be used to test the app and demonstrate its functionality.
