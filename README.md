# SIEM Log Anomaly Detector

## Project Overview
This project simulates an end-to-end security analysis workflow, from data generation to anomaly detection and visualization. It's built to demonstrate skills in cybersecurity, data analysis, and security operations.

## Key Skills Demonstrated
* **Python:** Used for generating realistic log data and developing custom anomaly detection logic with the `pandas` library.
* **Data Analysis:** Applied to identify patterns and anomalies in login activity.
* **Security Operations (SecOps):** Simulates the process of threat hunting and alert triage.
* **SIEM/Splunk:** Shows proficiency in ingesting log data, writing custom queries (SPL), and building interactive dashboards for threat visualization.

## Project Components
* **`generate_logs.py`**: A Python script that creates a simulated `login_logs.csv` file with a mix of normal and anomalous events.
* **`anomaly_detector.py`**: A Python script that analyzes the log data using predefined security rules to identify potential anomalies (e.g., failed logins from new IPs, brute-force attempts). The output is saved to `anomalies.csv`.
* **Splunk Dashboard**: The data is ingested into a Splunk instance and visualized on a dashboard, allowing a security analyst to easily monitor login activity and investigate alerts.

## How to Use This Project
1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/siem-anomaly-detector.git](https://github.com/your-username/siem-anomaly-detector.git)
    cd siem-anomaly-detector
    ```
2.  **Install Dependencies:**
    ```bash
    pip install pandas
    ```
3.  **Generate Logs:**
    ```bash
    python generate_logs.py
    ```
4.  **Run Anomaly Detection:**
    ```bash
    python anomaly_detector.py
    ```
This will produce the `anomalies.csv` file, which contains a list of flagged events. You can then upload this file, along with the original logs, into your SIEM of choice for visualization.

<img width="938" height="337" alt="splunk_dashboard_1" src="https://github.com/user-attachments/assets/010c79be-c6b4-458a-b585-87725583cb9f" />
<img width="932" height="284" alt="splunk_dashboard_2" src="https://github.com/user-attachments/assets/321eeba5-419f-4ddc-9663-8afed5f4e694" />
<img width="930" height="247" alt="splunk_dashboard_3" src="https://github.com/user-attachments/assets/00ee0d9c-657a-4b14-b089-05a33762e663" />




