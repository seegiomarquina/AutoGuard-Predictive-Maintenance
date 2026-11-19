# AutoGuard AI — Predictive Maintenance & Machine Failure Prediction

An end-to-end Machine Learning project that analyzes industrial sensor data and predicts potential machine failures using classification algorithms.

## Project Overview

Unexpected machine failures can cause production downtime, maintenance expenses, and operational disruptions.

AutoGuard AI explores how machine learning can help identify potential equipment failures using operating conditions and sensor measurements.

The project uses the AI4I 2020 Predictive Maintenance Dataset and compares multiple classification models to identify the most suitable approach.

**Project Type:** Machine Learning | Predictive Analytics | Industrial AI

## Problem Statement

Traditional maintenance approaches often depend on fixed maintenance schedules or reactive repairs.

The objective of this project is to develop a predictive maintenance prototype that uses machine sensor readings to estimate the likelihood of machine failure.

## Project Objectives

- Analyze industrial machine sensor data.
- Identify patterns associated with machine failures.
- Perform exploratory data analysis.
- Engineer additional predictive features.
- Train and compare classification models.
- Evaluate model performance using appropriate metrics.
- Explain model predictions using SHAP.
- Develop an interactive machine prediction interface.

## Dataset

**AI4I 2020 Predictive Maintenance Dataset**

Source: UCI Machine Learning Repository

https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset

The dataset contains 10,000 simulated industrial records and operating measurements.

### Main Features

| Feature | Description |
|---|---|
| Type | Product quality category |
| Air Temperature | Environmental temperature |
| Process Temperature | Operating process temperature |
| Rotational Speed | Machine RPM |
| Torque | Applied torque |
| Tool Wear | Tool usage duration |
| Machine Failure | Target variable |

The dataset also contains five failure-mode indicators, which are excluded from model training to prevent target leakage.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SHAP
- Joblib
- Google Colab

## Machine Learning Workflow

1. Automatic dataset acquisition.
2. Data cleaning and exploration.
3. Exploratory Data Analysis.
4. Feature engineering.
5. Train, validation and test splitting.
6. Logistic Regression model training.
7. Random Forest model training.
8. Validation-based model selection.
9. Classification threshold selection.
10. Final test evaluation.
11. SHAP explainability.
12. Interactive machine failure prediction.

## Feature Engineering

The project introduces additional features:

- Temperature Difference
- Mechanical Power
- Wear-Torque Interaction
- Temperature Ratio

These features provide additional representations of machine operating conditions.

## Models Implemented

### Logistic Regression

Used as a baseline classification approach.

### Random Forest

An ensemble learning algorithm used to capture nonlinear relationships between machine operating measurements and failure outcomes.

## Model Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- PR-AUC
- Confusion Matrix

### Actual Model Results

Replace the following placeholders with your actual Google Colab test results.

| Metric | Result |
|---|---|
| Selected Model | [Enter actual model] |
| Accuracy | [Enter actual result] |
| Precision | [Enter actual result] |
| Recall | [Enter actual result] |
| F1 Score | [Enter actual result] |
| ROC-AUC | [Enter actual result] |
| PR-AUC | [Enter actual result] |

No performance results are assumed or fabricated.

## Explainable AI

SHAP is used to investigate how different sensor features contribute to model predictions.

Permutation feature importance is also used to identify influential input variables.

## Project Visualizations

The project generates:

- Machine failure distribution.
- Failure distribution by product type.
- Sensor feature distributions.
- Feature correlation heatmap.
- Confusion matrix.
- ROC curve.
- Precision-recall curve.
- Feature importance chart.
- SHAP summary plot.

## Interactive Prediction

An interactive Google Colab interface allows users to enter:

- Product type.
- Air temperature.
- Process temperature.
- Rotational speed.
- Torque.
- Tool wear.

The trained model returns a failure probability and a prediction based on a validation-selected classification threshold.

## Repository Structure

```text
AutoGuard-AI-Predictive-Maintenance/
│
├── notebooks/
│   └── AutoGuard_AI_Day10.ipynb
│
├── src/
│   └── predict.py
│
├── models/
│
├── outputs/
│
├── reports/
│   └── PROJECT_REPORT.txt
│
├── requirements.txt
└── README.md
```

## How to Run

1. Clone the repository.

```bash
git clone https://github.com/YOUR_USERNAME/AutoGuard-AI-Predictive-Maintenance.git
```

2. Open the notebook in Google Colab.

3. Run the notebook cells in sequence.

4. The dataset is downloaded automatically.

5. Train the models and review the evaluation results.

6. Run the interactive prediction interface.

## Limitations

- The dataset contains simulated industrial sensor data.
- Model performance on real industrial equipment may differ.
- The prototype is not validated on actual automotive vehicle telemetry.
- Predictions should not replace professional equipment inspections or safety decisions.

## Future Improvements

- Real-time sensor data integration.
- FastAPI model-serving backend.
- Streamlit monitoring dashboard.
- Model drift monitoring.
- Additional anomaly detection algorithms.
- Validation on real industrial equipment data.

## Author

**Aditya Dhage**

Data Science & AI Enthusiast

GitHub: https://github.com/YOUR_USERNAME

## Acknowledgements

Dataset provided by the UCI Machine Learning Repository.

**Disclaimer:** This project is an educational and portfolio prototype developed for machine learning experimentation and predictive maintenance analysis.
