# Data Anomaly & Outlier Detection System 

A systematic machine learning benchmark designed to evaluate and compare the performance of different anomaly detection algorithms using the **PyOD** (Python Outlier Detection) library. This pipeline is highly applicable to identifying network intrusions, server metric spikes, or credit card fraud.

##  Project Overview
Anomaly detection suffers from extreme class imbalance (valid events far outnumber anomalous events). This project establishes a controlled benchmark environment to test how effectively distance-based and angle-based algorithms can isolate structural outliers in clustered geometric data.

##  Tech Stack & Methodology
* **Language & Ecosystem:** Python, PyOD, Scikit-Learn, Pandas, Matplotlib.
* **Data Engineering:** Constructed a synthetic evaluation dataset with a strict `0.1` contamination rate to simulate a 10% anomaly occurrence.
* **Algorithms Evaluated:**
  * **K-Nearest Neighbors (KNN):** Implemented as a distance-based baseline, measuring the Euclidean distance to the *k*-th nearest neighbor to flag isolated points.
  * **Angle-Based Outlier Detection (ABOD):** Utilized for its robustness in higher dimensions, identifying anomalies by analyzing the variance of angles between data points.

##  Evaluation & Results
* Both models were evaluated using Precision, Recall, and F1-Scores to account for class imbalance, rather than relying solely on raw accuracy.
* **KNN** proved highly computationally efficient and accurate for spherical data clusters.
* Visual decision boundaries were plotted to demonstrate how each algorithm mathematically segregates outliers from normal operational data.
