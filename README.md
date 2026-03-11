Electricity Theft Detection Using Machine Learning
Overview

Electricity theft is a major challenge faced by power distribution companies, leading to significant financial losses and instability in smart grid systems. This project proposes a machine learning-based Electricity Theft Detection System that analyzes smart meter consumption data to identify suspicious electricity usage patterns.

The system uses the SGCC (State Grid Corporation of China) smart meter dataset and applies data preprocessing, time-series feature engineering, and a Random Forest classifier to detect abnormal consumption behavior. The model classifies electricity usage into three categories:

Normal

Potential Theft

Abnormal

Additionally, the system performs transformer-wise and location-wise risk analysis to identify high-risk areas and assist utility companies in prioritizing inspections.

Project Features

Data preprocessing and missing value handling

Conversion of raw consumption data into time-series format

Feature extraction using Previous Consumption and Drop Percentage

Rule-based labeling for generating class labels

Random Forest classifier for multi-class classification

Model evaluation using Accuracy, Precision, Recall, and F1-score

Confusion Matrix visualization

Transformer-wise and location-wise analysis for identifying high-risk regions

Dataset

The project uses the SGCC Smart Meter Dataset, which contains electricity consumption records of multiple consumers across different time periods.

Since the dataset does not contain theft labels, a rule-based labeling method is implemented based on sudden consumption drops.

Methodology

The project follows these main steps:

Data Preprocessing

Load dataset

Handle missing values

Convert data into time-series format

Feature Engineering

Calculate Previous Consumption

Compute Drop Percentage

Label Generation

Apply rule-based thresholds

Categorize consumers into Normal, Potential Theft, and Abnormal

Model Training

Train a Random Forest classifier

Split dataset into 80% training and 20% testing

Model Evaluation

Accuracy

Precision

Recall

F1-score

Confusion Matrix

Risk Analysis

Transformer-wise risk detection

Location-wise risk analysis

Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

Google Colab / Jupyter Notebook

Results

The Random Forest classifier achieved approximately:

Accuracy: ~94%

Precision: ~0.90

Recall: ~0.89

F1-score: ~0.90

The model effectively identifies abnormal electricity consumption behavior and helps detect potential electricity theft cases.

Project Structure
Electricity-Theft-Detection/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── electricity_theft_detection.ipynb
│
├── src/
│   └── model_training.py
│
├── results/
│   └── confusion_matrix.png
│
└── README.md
Future Improvements

Integration with real-time smart grid monitoring systems

Use of deep learning models (LSTM, Transformers) for improved temporal pattern detection

Deployment using IoT-enabled smart meters

Implementation of Explainable AI (XAI) techniques

Testing across multiple regional datasets

Applications

Electricity theft detection in smart grids

Reducing non-technical losses in power distribution

Supporting utility inspection planning

Improving energy monitoring and grid stability

Author

Bhanu Prakash Sunchu
B.Tech – CSE (Artificial Intelligence & Machine Learning)
