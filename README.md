# A Safety-Aware Edge AI Agent for Real-Time Smart Irrigation Using IoT Sensor Fusion

![Project](https://img.shields.io/badge/Project-Final%20Year%20Project-blue)
![Domain](https://img.shields.io/badge/Domain-AI%20%7C%20IoT%20%7C%20Agriculture-green)
![Status](https://img.shields.io/badge/Status-Research%20%26%20Development-orange)
![Language](https://img.shields.io/badge/Language-Python-yellow)

## 📌 Project Overview

This project proposes a safety-aware Edge AI irrigation system that combines Internet of Things (IoT), Machine Learning, anomaly detection, and AI-based decision-making to improve irrigation management.

The system collects real-time environmental data through multiple sensors, identifies unreliable sensor readings, predicts irrigation requirements, and generates irrigation decisions.

Before executing any action, an independent deterministic safety validator checks the proposed decision to prevent unsafe pump operations.

The system is designed to operate locally using Edge AI processing on a Raspberry Pi, with an ESP32 handling sensor data acquisition.

## 🎯 Research Objectives

- Develop an IoT-based smart irrigation prototype.
- Collect real-time soil and environmental sensor measurements.
- Implement sensor data preprocessing and validation.
- Detect abnormal sensor readings using anomaly detection.
- Predict irrigation requirements using Machine Learning.
- Develop an AI decision-making agent.
- Implement an independent safety validation mechanism.
- Support human approval when uncertainty is high.
- Evaluate the system under normal and faulty sensor conditions.

## 🏗️ Proposed System Architecture

**Main workflow:**

1. Sensor Data Acquisition — Soil moisture, temperature, humidity, light intensity, and water level.
2. IoT Communication — ESP32 transmits sensor readings using MQTT.
3. Edge Processing — Raspberry Pi processes incoming sensor data.
4. Data Validation — Handle missing, noisy, delayed, and faulty readings.
5. Anomaly Detection — Isolation Forest identifies abnormal readings.
6. Irrigation Prediction — Random Forest and Logistic Regression predict irrigation requirements.
7. AI Decision Agent — Combines sensor context, predictions, and confidence.
8. Safety Validation — Independent rules approve or reject proposed actions.
9. Actuator Control — Approved decisions control the relay and water pump.
10. Monitoring — Dashboard displays real-time data, decisions, and alerts.

## 🧠 Machine Learning Components

| Algorithm | Purpose |
|---|---|
| Logistic Regression | Baseline irrigation prediction |
| Random Forest | Irrigation requirement prediction |
| Isolation Forest | Sensor anomaly detection |

## 🛠️ Technologies and Tools

**Programming and Data Science**
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

**IoT and Hardware**
- ESP32
- Raspberry Pi
- MQTT
- Soil Moisture Sensor
- DHT22 Temperature and Humidity Sensor
- Light Sensor
- Water-Level Sensor
- Relay Module
- Mini Water Pump

**Dashboard and Development**
- Streamlit
- Jupyter Notebook
- VS Code
- Git and GitHub

## 🧪 Research and Evaluation

The proposed system will be evaluated under the following conditions:

- Normal sensor operation
- Noisy sensor readings
- Missing sensor values
- Delayed sensor data
- Faulty sensor readings
- Contradictory sensor measurements

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- Anomaly Detection Performance
- Water Consumption
- Unsafe Action Prevention
- Decision-making Latency
- Edge Device Resource Usage

The proposed safety-aware system will be compared with a conventional rule-based controller and an unguarded AI model.

## 📂 Repository Structure

```text
smart-irrigation-edge-ai/
├── research/
├── dataset/
├── notebooks/
├── src/
├── iot/
├── agent/
├── dashboard/
├── experiments/
├── docs/system-architecture.png/
└── tests/
```

## 👥 Project Team

| Member | Registration No. |
|---|---|
| Arosh Khan | 23pwdsc0106 |
| Muhammad Dawood Hussain | 23pwdsc0121 |
| Shahzainulhaq | 23pwdsc0135 |

**Supervisor:** Muhammad Naeem Khan

**Department:** Computer Science & Information Technology  
**University:** University of Engineering & Technology, Peshawar, Pakistan

## 🚧 Current Development Status

This repository is being used to manage the research, implementation, experiments, and documentation of the Final Year Project.

Implementation milestones and experimental results will be updated as development progresses.

## 🔬 Research Contribution

The primary research focus is to investigate whether sensor reliability assessment and independent safety validation can improve the reliability of AI-driven irrigation decisions under uncertain and faulty sensor conditions.
