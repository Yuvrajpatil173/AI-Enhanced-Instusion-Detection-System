# Cyber Security AI Enhanced Intrusion Detection System

## Overview

Cyber Security AI Enhanced Intrusion Detection System is a Machine Learning based web application that detects malicious web attacks from network traffic features.

The system uses a trained Random Forest Classifier to classify incoming traffic into one of the following categories:

* BENIGN
* Web Attack – Brute Force
* Web Attack – SQL Injection
* Web Attack – XSS

The application provides an interactive web interface where users can enter network flow parameters and instantly receive attack predictions.

---

## Features

* Machine Learning based Intrusion Detection
* Random Forest Classification Model
* Real-time Attack Prediction
* Detection of Multiple Web Attack Types
* Modern Cybersecurity-Themed User Interface
* Flask Web Framework Integration
* Easy Deployment and Testing

---

## Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Python
* Flask

### Machine Learning

* Scikit-Learn
* Random Forest Classifier
* NumPy
* Joblib

### Dataset

* Web Attack Network Traffic Dataset

---

## Project Structure

```text
CYBER_PROJECT/
│
├── app.py
├── random_forest_model_4_features.joblib
├── web_attacks_balanced.csv
│
├── templates/
│   └── index.html
│
├── static/
│   └── assets/
│
└── README.md
```

---

## Input Features

The model uses the following network traffic features:

1. Flow Duration
2. Total Forward Packets
3. Total Backward Packets
4. Total Length of Forward Packets

---

## Output Classes

The model predicts one of the following classes:

| Class                      | Description                 |
| -------------------------- | --------------------------- |
| BENIGN                     | Normal network traffic      |
| Web Attack – Brute Force   | Brute Force Attack          |
| Web Attack – SQL Injection | SQL Injection Attack        |
| Web Attack – XSS           | Cross-Site Scripting Attack |

---

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd CYBER_PROJECT
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Virtual Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install flask numpy pandas scikit-learn joblib imbalanced-learn
```

---

## Run Application

```bash
python app.py
```

Application will start at:

```text
http://127.0.0.1:5000
```

Open the URL in your browser.

---

## How It Works

1. User enters network traffic parameters.
2. Flask receives the input values.
3. Input data is converted into a NumPy array.
4. Random Forest model processes the features.
5. Model predicts the traffic category.
6. Prediction result is displayed on the web interface.

---

## Sample Prediction

Input:

```text
Flow Duration: 62015
Total Fwd Packets: 2
Total Backward Packets: 0
Total Length of Fwd Packets: 12
```

Output:

```text
BENIGN
```

---

## Future Enhancements

* Deep Learning Based Detection
* Real-Time Packet Monitoring
* Live Network Traffic Analysis
* Attack Visualization Dashboard
* Threat Severity Scoring
* Database Integration
* Cloud Deployment

---

## Author

Rushikesh Jadhav

---

## License

This project is developed for educational and academic purposes.
