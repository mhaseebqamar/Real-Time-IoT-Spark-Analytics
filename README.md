# Real-Time IoT Sensor Analytics & Anomaly Detection
### Predictive Maintenance Pipeline with PySpark & Isolation Forest

## 📌 Project Overview
This project implements a scalable, big-data monitoring pipeline designed for **Industrial IoT (IIoT)** environments. Utilizing **PySpark on Databricks**, the system processes high-frequency streams from Temperature, Pressure, and Vibration sensors to identify hardware irregularities and environmental instabilities.

The primary goal is to transition from reactive repairs to a **Predictive Maintenance** strategy by detecting subtle sensor anomalies before they lead to catastrophic equipment failure.

---

## 🛠️ Technical Stack & Engineering
* **Engine:** PySpark (Spark SQL & MLlib)
* **Platform:** Databricks (Cloud-native Distributed Computing)
* **Core Algorithm:** **Isolation Forest** (Unsupervised Anomaly Detection)
* **Data Context:** Multi-sensor streams (Temperature, Pressure, Vibration)

### Engineering Highlights:
* **High-Frequency Data Ingestion:** Developed structured Spark schemas to handle large-scale concurrent sensor streams.
* **Model Precision:** The Isolation Forest model achieved a **95% anomaly detection rate** with a highly optimized false-positive rate of ~3%.
* **Temporal & Geospatial Analysis:** Engineered logic to track failure rates across specific building locations and time-of-day windows.

---

## 🚀 Key Insights & Findings
The analytics engine uncovered several critical patterns that drive immediate business value:

* **Anomaly Distribution:** Flagged **8% of all readings** as anomalous, with the majority (60%) identified as high-temperature spikes (>35°C).
* **Location Hotspots:** Identified **Building_A** as a high-risk zone with a 10% failure rate, significantly higher than the fleet average.
* **Hardware Lifecycle Analysis:** Discovered that **Sensor_v1** devices fail 2x more often than newer versions, providing data-backed justification for a hardware upgrade.
* **Temporal Patterns:** Detected a consistent anomaly cluster between **2-00 AM and 4:00 AM**, pointing toward systemic HVAC/Climate Control issues during off-peak hours.

---

## 💼 Business & Operational Impact
1.  **Predictive Maintenance:** Integrated the Isolation Forest model to act as an early-warning system, reducing unplanned downtime and maintenance costs.
2.  **Asset Optimization:** Provided specific recommendations for building-level sensor replacements based on historical failure data.
3.  **Energy Efficiency:** Identified climate control instabilities during off-peak hours, offering a path to optimize HVAC performance and reduce energy waste.

---

## 📂 Repository Structure
* `IoT_Anomaly_Detection.ipynb`: Full PySpark pipeline from data cleaning to model deployment.
* `visualizations/`: Heatmaps showing anomaly clusters by time and location.
* `docs/`: Technical summary of the Isolation Forest hyperparameter tuning.
