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
```
Results

Model accuracy:

98.15%

Most important feature:

Tool wear [min]
IBM Cloud Deployment

The trained model was stored as a Watson Machine Learning model asset and deployed as an online backend service using IBM watsonx.ai Runtime.

Deployment details:

Deployment Type: Online
Deployment Status: Deployed
Prediction Type: Multiclass Classification
Sample Prediction

Sample input:

{
  "input_data": [
    {
      "fields": [
        "Type",
        "Air temperature [K]",
        "Process temperature [K]",
        "Rotational speed [rpm]",
        "Torque [Nm]",
        "Tool wear [min]"
      ],
      "values": [
        [0, 298.1, 308.6, 1551, 42.8, 0]
      ]
    }
  ]
}

Output:

Prediction: No Failure
Project Workflow
Dataset Upload
        ↓
Data Preprocessing
        ↓
Label Encoding
        ↓
Train-Test Split
        ↓
Random Forest Model Training
        ↓
Model Evaluation
        ↓
Watson Machine Learning Deployment
        ↓
Online Prediction Testing
Security Note

IBM API keys, project tokens, and access credentials are removed from this repository for security reasons.

Conclusion

This project successfully demonstrates a predictive maintenance system for industrial machinery. The deployed backend model can classify machine failure types and support preventive maintenance decisions.


