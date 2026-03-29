# 🏭 AI-Powered Predictive Maintenance Engine

An end-to-end Machine Learning pipeline designed to predict machine failures before they occur. By analyzing real-time sensor data (RPM, Torque, Temperature, Tool Wear), this system acts as an early warning mechanism for industrial equipment, minimizing downtime and maintenance costs.

## 🚀 Key Engineering Features

* **Data Preprocessing & Feature Engineering:**
  * Processed the local `ai4i2020.csv` dataset, stripping non-predictive identifiers (UDI, Product ID) to reduce noise.
  * Encoded categorical equipment quality types (L, M, H) into numerical values for algorithmic processing.
* **Exploratory Data Analysis (EDA):** * Visualized sensor correlations using `Seaborn` heatmaps, validating physical principles (e.g., the strong negative correlation between Rotational Speed and Torque).
* **Machine Learning Architecture:**
  * Implemented a **Random Forest Classifier** (`scikit-learn`) to detect complex, non-linear failure patterns.
  * Applied `class_weight='balanced'` to explicitly handle the severe class imbalance typical in real-world anomaly detection scenarios (where failures are rare compared to normal operations).
* **Real-time Inference Simulation:** * Developed a testing module that accepts live sensor arrays and instantly classifies the machine state as "Normal" or "Failure Expected".

## 🛠️ Tech Stack

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Language** | Python 3.x | Core Logic |
| **Data Processing** | Pandas, NumPy | Local CSV parsing, cleaning, and manipulation |
| **Machine Learning** | Scikit-Learn | Random Forest Classification & Performance Metrics |
| **Visualization** | Matplotlib, Seaborn | Sensor correlation and failure heatmaps |

## 📊 Business Value
Predictive maintenance shifts industrial operations from a reactive ("fix it when it breaks") to a proactive model. This AI engine helps in:
1. Preventing catastrophic equipment failures.
2. Optimizing the lifecycle of machine parts.
3. Ensuring continuous production lines in heavy industries and defense technologies.

## 👨‍💻 About the Developer
**Muhammed Emin**
* **Software Engineering Student** focusing on Data Science, Machine Learning pipelines, and creating scalable, data-driven engineering solutions.
