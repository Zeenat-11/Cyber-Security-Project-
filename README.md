# AI-Enhanced Intrusion Detection System

This project implements an AI-powered Intrusion Detection System (IDS) that classifies network traffic to detect web attacks. It uses a Random Forest classifier with SMOTE for handling imbalanced data and provides a web interface built with Flask for easy predictions and deployment.

---

## Features

- Data preprocessing and handling class imbalance using SMOTE.
- Training a Random Forest classifier with feature scaling.
- Saving and loading the model pipeline for inference.
- Command-line scripts for training and prediction.
- Flask web framework to serve the application backend and provide REST APIs or web pages.

---

## Project Files

- `train_model_pipeline.py` — Train and save the model pipeline.
- `predict_pipeline.py` — Predict on new datasets using the saved pipeline.
- `flask_app.py` — Flask web application backend.
- `README.md` — Project documentation.
- `requirements.txt` — Python dependencies (optional).
- Sample CSV files (optional, not included).

---

## Installation

Make sure you have Python 3.7 or higher installed. Then install the required packages:

```bash
pip install pandas scikit-learn imbalanced-learn joblib flask
