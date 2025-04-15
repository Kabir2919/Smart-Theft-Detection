# ⚡ Smart Energy Theft Detection

## 🔍 Overview  
This project aims to detect electricity theft using smart meters and intelligent deep learning techniques. It addresses **non-technical losses (NTL)** like power theft and irregular billing, which cause major economic setbacks. Leveraging **federated learning** and **AI-driven anomaly detection**, we offer a novel approach that ensures both efficiency and data privacy.

---

## 🌐 Introduction  
A **Smart Grid** connects intelligent sensors and meters to central servers or cloud platforms via wired or wireless networks. It enhances energy efficiency through:

- **Real-time monitoring**
- **Dynamic load scheduling**
- **Forecasting user behavior**

This integration evolves into what’s known as the **Energy Internet (EI)**. At its core, **Advanced Metering Infrastructure (AMI)** enables utilities to gather fine-grained energy usage data, which is crucial for demand response and forecasting.

However, Smart Grids face challenges like:

- **High deployment costs**
- **Cybersecurity risks**
- **Significant losses from NTL** (power theft, billing irregularities)

To address these, our solution applies:

- **AI and Deep Learning** to identify abnormal consumption patterns  
- **Federated Learning (FL)** for privacy-preserving model training  
- **Game Theory** for modeling behavior between providers and malicious users  

---

## 📊 Dataset Used

- **Source**: [Mendeley Data](https://data.mendeley.com/datasets/c3c7329tjj/3)  
- **Size**: 58,565 samples (we used 20,000 for analysis)  
- **Details**: Includes normal and simulated electricity theft scenarios  
- **Purpose**: Designed for benchmarking ML-based classification in smart grid environments  

---

## 🚩 Anomalies Predicted

### 🔴 Abnormal Consumption Patterns

- **Red Dots**: Indicate spikes or drops deviating from regular usage  
- **Example**:  
  - *Spike at hour 200* → Possible unauthorized tapping  
  - *Drop at hour 800* → Potential meter tampering or bypassing  

---

### ✅ Normal But High Usage  
A high value (e.g., 200 kWh at 5:00 AM) may **not be flagged** due to:

- **Threshold-Based Detection**: May fall within allowed statistical range  
  - *Mean: 100 kWh, Std Dev: 50 → Threshold = 200 kWh*  
- **Contextual Variability**: Usage might be typical during early hours in some scenarios  
