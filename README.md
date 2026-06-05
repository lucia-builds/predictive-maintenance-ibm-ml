# predictive-maintenance-ibm-ml
# Predictive Maintenance of Industrial Machinery

This project predicts possible machine failures using machine learning. It uses machine sensor data such as air temperature, process temperature, rotational speed, torque, tool wear, and machine type to classify the failure type.

## Problem Statement

Develop a predictive maintenance model for industrial machinery to anticipate failures before they occur. The goal is to reduce downtime and operational costs by predicting machine failure types from sensor data.

## Dataset

Dataset used: Machine Predictive Maintenance Classification dataset from Kaggle.

Main columns:
- UDI
- Product ID
- Type
- Air temperature [K]
- Process temperature [K]
- Rotational speed [rpm]
- Torque [Nm]
- Tool wear [min]
- Target
- Failure Type

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- IBM watsonx.ai Studio
- IBM Cloud Object Storage
- IBM watsonx.ai Runtime / Watson Machine Learning

## Machine Learning Model

Model used:

```text
Random Forest Classifier
