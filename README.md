# 🔍 Synthetic Anomaly Injection and Detection Benchmarking on Electricity Time-Series Data

This repository is built to simulate and benchmark synthetic anomalies (specifically **Types 2, 3, and 4**) in electricity consumption time-series data, based on the **NNG-Mix** framework. The aim is to inject controlled disruptions in the dataset and evaluate the robustness of anomaly detection techniques.

---

## 📌 Overview

This project is divided into three major components:

1. **Anomaly Injection**  
   Code to inject synthetic anomalies—particularly **Type 3 (Extreme Negative Values)**—into the dataset.

2. **Dataset Preparation**  
   Tools for preprocessing, imputing missing values, extracting trends, and formatting the data.

3. **Benchmarking & Visualization**  
   Implementation of classical anomaly detection algorithms with visual evaluation and performance plots.

---

## 🚀 Features

- ✅ **Type 3 Injection** (Extreme Negative Values)
- 📈 **Kalman & Seasonal Decomposition Imputation**
- 🌡️ **Anomaly Trend Visualizations** (as HTML heatmaps)
- 🧪 **Detection Algorithms Implemented**:
  - IQR (Interquartile Range)
  - LOF (Local Outlier Factor)
  - Isolation Forest
  - Modified Z-Score

---

## 📁 Directory Structure

```bash
.
├── benchmarking_code/
│   ├── src/                     # Jupyter notebooks implementing detection algorithms (IQR, LOF, etc.)
│   └── plots/                   # Visual output for each detection method (e.g., heatmaps, score plots)
│
├── dataset_prep/
│   ├── src/                     # Dataset cleaning, transformation, and preprocessing (V1 & V2)
│   └── visualization/           # HTML-based trend visualizations and anomaly heatmaps
│
├── injection_code/
│   └── src/                     # Code for injecting synthetic anomalies (currently Type 3)
│
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
