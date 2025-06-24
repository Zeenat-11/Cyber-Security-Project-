
# 🚨 AI-Enhanced Intrusion Detection System (IDS)

This project implements a robust AI-powered Intrusion Detection System that detects and classifies network intrusions using machine learning techniques. It leverages a **Random Forest classifier** and handles **imbalanced datasets** using **SMOTE** (Synthetic Minority Oversampling Technique). A user-friendly **Flask web interface** enables real-time predictions and deployment.

---

## 🔍 Features

- ✅ Preprocessing of network traffic datasets
- ✅ Handling class imbalance using SMOTE
- ✅ Training a Random Forest classifier
- ✅ Saving and reloading the full model pipeline using `joblib`
- ✅ Web-based prediction UI using Flask
- ✅ RESTful prediction API
- ✅ Easy integration and deployment-ready structure

---

## 🗂️ Project Structure

```bash
├── train_model_pipeline.py      # Training script
├── predict_pipeline.py          # Command-line prediction script
├── flask_app.py                 # Flask-based web application
├── templates/
│   └── index.html               # Web UI for prediction
├── static/                      # (Optional) Static files for web styling
├── model_pipeline.pkl          # Saved model pipeline
├── requirements.txt             # Python dependencies
├── README.md                    # Project documentation
└── data/
    ├── train.csv                # Training dataset (not included)
    └── test.csv                 # Testing dataset (not included)
````

---

## ⚙️ Installation

Make sure you have **Python 3.7+** installed.

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is not available, manually install dependencies:

```bash
pip install pandas scikit-learn imbalanced-learn joblib flask
```

---

## 🏋️‍♂️ Model Training

Train the Random Forest model with your dataset:

```bash
python train_model_pipeline.py
```

> Output: `model_pipeline.pkl` (saved pipeline including preprocessing and classifier)

---


## 🌐 Web Interface (Flask App)

Run the Flask server:

```bash
python flask_app.py
```

Then visit: [http://127.0.0.1:5000](http://127.0.0.1:5000)
You can either enter inputs manually or upload a CSV file for prediction.

---

## 🧠 Model

* Classifier: `RandomForestClassifier`
* Preprocessing: `StandardScaler`
* Imbalance Handling: `SMOTE`
* Evaluation Metrics: Accuracy, Precision, Recall, F1 Score

---

## 📁 Example Input Fields

| Feature                  | Description                        |
| ------------------------ | ---------------------------------- |
| Flow Duration            | Duration of the network flow       |
| Total Fwd Packets        | Total packets sent in forward dir  |
| Total Backward Packets   | Total packets sent in reverse dir  |
| Total Length Fwd Packets | Total length of forward packets    |
| ...                      | Extend with other network features |


  
GitHub  
https://github.com/Zeenat-11/Cyber-Security-Project-.git 
 
Project Demo Link 
https://drive.google.com/file/d/1B4PAPswbIr9JTFYW
2ytGlosUWN1y_gP/view?usp=drive_link  
