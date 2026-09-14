# 📡 Telecom Network Failure & Anomaly Predictor

> A machine learning pipeline for analyzing 5G network telemetry, detecting anomalous behavior, and estimating network failure risk using time-series network KPIs.

---

## 🔍 Overview

Modern 5G networks generate large volumes of telemetry across different layers of the network. Changes in network KPIs such as radio quality, throughput, latency, and error rates can indicate abnormal network behavior and potential service degradation.

This project aims to develop a machine learning-based system that analyzes multivariate 5G network telemetry, identifies abnormal behavior, and provides a network health and failure-risk assessment.

The project combines **time-series analysis, machine learning, feature engineering, anomaly detection, and interactive visualization** into a modular ML pipeline.

---

## 🎯 Objectives

- Analyze multivariate 5G network KPI time-series data
- Perform data preprocessing and exploratory data analysis
- Extract temporal and statistical features from network telemetry
- Detect and classify anomalous network behavior
- Compare traditional machine learning and temporal models
- Identify network KPIs associated with abnormal behavior
- Generate a network health / failure-risk score
- Build an interactive monitoring dashboard
- Develop a modular and testable ML pipeline

---

## 🧠 System Architecture

```text
                 5G Network Telemetry
                         │
                         ▼
              Data Loading & Validation
                         │
                         ▼
                  Data Preprocessing
                         │
                         ▼
              Exploratory Data Analysis
                         │
                         ▼
             Temporal Feature Engineering
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
     Rolling Stats    Lag Features   Trend Analysis
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                  ML Model Layer
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
    Logistic Reg.   Random Forest    XGBoost
                         │
                         ▼
                       LSTM
                         │
                         ▼
              Anomaly / Risk Prediction
                         │
                         ▼
              Model Evaluation & Analysis
                         │
                         ▼
               Streamlit Monitoring UI
