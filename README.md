Cybersecurity – Suspicious Web Threat Interactions
📌 Overview

During my internship, I worked on this project to analyze AWS CloudWatch web traffic logs and detect suspicious or malicious interactions. The dataset contained details like source and destination IPs, ports, bytes transferred, countries, and rule names.

The main aim of this project was to build a complete machine learning pipeline that could automatically identify unusual patterns in the traffic and help in classifying suspicious requests from normal ones.

🔹 What I Did

Data Cleaning & Preprocessing
I started by removing duplicate entries, handling missing values, and converting time-related fields into proper datetime format. This helped in making the data more reliable for analysis.

Feature Engineering
I created new features such as session duration, average packet size, and throughput. I also added a binary label is_suspicious which marked whether the request looked suspicious or not.

Exploratory Data Analysis (EDA)
To understand the data better, I plotted histograms of bytes in and out, checked which ports and protocols were most used, and visualized country-wise traffic. I also created time-series plots to see how traffic changed over time, a correlation heatmap to find relationships between variables, and even a small network graph to see connections between IPs.

Anomaly Detection
I applied Isolation Forest and Local Outlier Factor to detect unusual traffic patterns. These models helped in pointing out potential attacks hidden in normal traffic.

Classification Models
For supervised learning, I trained a RandomForest classifier and also experimented with deep learning models like a Multi-Layer Perceptron (MLP) and Conv1D neural network.

Evaluation
I measured performance using accuracy, precision, recall, F1-score, and ROC-AUC. RandomForest performed the best, achieving more than 90% accuracy.

🔹 Results

This project gave me a good understanding of how real-world cybersecurity data can be processed and analyzed using machine learning. I also learned how anomaly detection and classification models can complement each other in detecting suspicious web threats.
