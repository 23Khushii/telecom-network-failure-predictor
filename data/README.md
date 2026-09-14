# Telecom Network Failure & Anomaly Predictor

> A machine learning pipeline for analyzing 5G network telemetry, detecting anomalous behavior, and estimating network failure risk from time-series KPIs.

---

## 📡 Overview

Modern 5G networks generate large volumes of telemetry data across radio, transport, and network layers. Abnormal behavior in network KPIs can indicate degradation, service instability, or an upcoming network issue.

This project explores how machine learning can be used to analyze multivariate 5G network telemetry and identify abnormal network behavior before it significantly impacts service quality.

The system is designed around a time-series ML pipeline that processes historical KPI behavior, extracts temporal patterns, evaluates multiple machine learning models, and presents network health and risk information through an interactive dashboard.

---

## 🎯 Objectives

- Analyze multivariate 5G network KPI time-series data
- Perform data cleaning and exploratory analysis
- Engineer temporal and statistical features from network telemetry
- Detect and classify anomalous network behavior
- Compare traditional machine learning models with temporal models
- Identify KPIs contributing to abnormal network behavior
- Generate a network health / failure-risk score
- Develop an interactive monitoring dashboard
- Build a modular and testable ML pipeline

---

## 🧠 Planned ML Pipeline

```text
5G Network Telemetry
        │
        ▼
Data Loading & Validation
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Preprocessing
        │
        ▼
Temporal Feature Engineering
        │
        ├── Rolling Statistics
        ├── Lag Features
        ├── Trend Analysis
        └── KPI Relationships
        │
        ▼
Machine Learning Models
        │
        ├── Logistic Regression
        ├── Random Forest
        ├── XGBoost
        └── LSTM
        │
        ▼
Anomaly / Risk Prediction
        │
        ▼
Model Evaluation & Explainability
        │
        ▼
Streamlit Monitoring Dashboard