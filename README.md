<h1 align="center">Flight Cancellations Prediction Using SVM and PySpark</h1>

<p align="center">
Predicting flight cancellations using distributed machine learning with PySpark and Hadoop, achieving 98% accuracy through large-scale data processing and model optimization.
</p>

***

## 📘 Table of Contents
- [About the Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#tech-stack)
- [Dataset](#-dataset)
- [Architecture](#-architecture)
- [Methodology](#-methodology)
- [Results](#-results)
- [Future Work](#-future-work)
- [Getting Started](#getting-started)

***

## 🧠 About the Project
This project focuses on **predicting flight cancellations** by developing a machine learning model using **Support Vector Machines (SVM)** implemented with **PySpark**. The goal is to leverage **Hadoop distributed computing** to process millions of flight records efficiently and generate actionable insights for proactive airline management.

The project demonstrates how **Big Data technologies** can be harnessed for scalability, speed, and precision in predictive analytics.

***

## ✨ Features
- Distributed data processing using Hadoop with **1 master** and **2 worker nodes**  
- Implementation of **SVM classification model** in **PySpark**  
- Feature selection, normalization, and preprocessing for improved model performance  
- Visualization of CPU usage and Spark cluster monitoring  
- Tackles Big Data V’s — **Volume, Velocity, Veracity, Variability, Value**  
- Achieved **98% model accuracy** with a **recall of 1.00**

***

## Tech Stack
- **Languages:** Python 3.12  
- **Frameworks:** Apache Spark, Hadoop  
- **Libraries:** PySpark, Pandas, NumPy, Matplotlib  
- **Cluster Setup:**
  - Master Node: Windows 11, Intel Core Ultra 5, 16 GB RAM  
  - Worker Nodes: macOS Sequoia 15.0, 8–16 GB RAM  
- **Versions:** Hadoop 3.3.6, OpenJDK 1.8.0  

***

## 📊 Dataset
- **Source:** Kaggle Flight Cancellations Dataset  
- **Attributes Include:** Flight Number, Airline, Departure Time, Arrival Time, Delay, Cancellation Reason, etc.  
- **Preprocessing Steps:**
  - Handling missing values  
  - Feature encoding and normalization  
  - Splitting data into train/test sets  

***

## 🧩 Architecture
```
           ┌─────────────────────────────┐
           │        Flight Data          │
           └────────────┬────────────────┘
                        │
              Data Preprocessing
                        │
                 PySpark SVM Model
                        │
             ┌──────────┴──────────┐
             │                     │
        Model Training        Model Evaluation
             │                     │
        Prediction Output      Accuracy Reports
```

***

## 🧪 Methodology
1. **Data Preprocessing:** Cleaning and normalization of flight records.  
2. **Model Training:** Implemented SVM algorithm using PySpark.  
3. **Cluster Utilization:** Distributed computation managed by Hadoop YARN.  
4. **Model Evaluation:** Metrics — Accuracy, Precision, Recall, F1 Score.  
5. **Visualization:** CPU and Spark Dashboard monitoring for performance tracking.

***

## 📈 Results
| Metric | Score |
|:-------|:------|
| Accuracy | 98% |
| Precision | 0.98 |
| Recall | 1.00 |

The high recall indicates the model’s strong ability to detect potential cancellations while minimizing false negatives.

***

## 🚀 Future Work
- Comparative analysis with Decision Trees and Neural Networks.  
- Incorporating **real-time data streams** for live cancellation prediction.  
- Integration with **airline decision systems** for automated scheduling.  

***

## Getting Started
### Prerequisites
- Python 3.12  
- Hadoop 3.3.6 configured cluster  
- Apache Spark setup

### Installation
```bash
git clone https://github.com/<your-username>/Flight-Cancellations-Prediction.git
cd Flight-Cancellations-Prediction
pip install -r requirements.txt
```

### Run the Project
```bash
spark-submit scripts/train_svm_model.py
```

### View Cluster Dashboard
Navigate to  
`http://<master-node-ip>:8080` to monitor Spark jobs and performance.

***

⭐ **If you found this project insightful, give it a star!**  
