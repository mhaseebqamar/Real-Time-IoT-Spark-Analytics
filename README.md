# Real-Time IoT Sensor Analytics & Anomaly Detection (PySpark)

📌 Project Overview

This project leverages PySpark on Databricks to build a scalable monitoring and anomaly detection pipeline for industrial IoT sensors. By analyzing high-frequency data from Temperature, Pressure, and Vibration sensors, the system identifies critical hardware irregularities and environmental instabilities to drive predictive maintenance strategies.

🛠️ Technical Stack

Language: Python (PySpark)

Platform: Databricks

Machine Learning: Isolation Forest (95% anomaly detection rate)

Libraries: Pandas, NumPy, Matplotlib, Seaborn

🚀 Key Features

Big Data Ingestion: Processed large-scale sensor streams using structured Spark schemas.

Advanced Anomaly Detection: Implemented an Isolation Forest model that successfully identified 95% of temperature anomalies with a low false-positive rate (~3%).

Temporal & Geospatial Analysis: Identified specific "Building-level" failure rates and hourly patterns (2-4 AM) linked to HVAC instability.

Predictive Insights: Correlated high humidity with temperature instability to refine alert thresholds.

📈 Key Insights & Findings

Anomaly Distribution: Approximately 8% of all readings were flagged as anomalous, with 60% being high-temperature spikes (>35°C).

Location Hotspots: Building_A exhibited the highest failure rate (~10%), leading to a recommendation for immediate sensor replacement.

Hardware Lifecycle: Data revealed that Sensor_v1 devices have a 2x higher failure rate than newer versions, justifying a fleet-wide upgrade.

Temporal Patterns: Significant anomalies were detected between 2-4 AM, suggesting systemic issues with climate control systems during off-peak hours.

💼 Business Recommendations

Immediate: Deploy a real-time alerting system and prioritize Building_A for maintenance to mitigate hardware risk.

Strategic: Transition from reactive to Predictive Maintenance by integrating the Isolation Forest model with existing Building Management Systems (BMS).

Optimization: Investigate the 2-4 AM anomaly cluster to optimize energy usage and HVAC performance.
