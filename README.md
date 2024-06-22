
# Equipment Failure Detection Using Machine Learning

### Overview

This project focuses on predicting equipment failures using machine learning techniques. The dataset used in this project contains various operational parameters and failure types. The goal is to build predictive models that can accurately identify equipment failures based on these parameters.

### Table of Contents

1. [Introduction](#introduction)
2. [Objectives](#objectives)
3. [Dataset](#dataset)
4. [Methodology](#methodology)
5. [Results](#results)
6. [Conclusion](#conclusion)
7. [Installation and Usage](#installation-and-usage)

### Introduction

Predictive maintenance is essential in industrial settings to preemptively address potential equipment failures, thus minimizing downtime and maintenance costs. Machine learning models are employed to analyze historical data and predict failures based on operational parameters.

### Objectives

- **Data Exploration:** Understand the dataset structure, key features, and assess data quality.
- **Preprocessing:** Handle missing values, visualize data distributions, and normalize features.
- **Model Training:** Train and evaluate multiple classification models to predict equipment failures.
- **Performance Evaluation:** Measure model accuracy and compare performance to identify the most effective predictive model.
- **Recommendations:** Provide insights to optimize maintenance schedules and improve operational efficiency based on model findings.

### Dataset

The dataset (`predictive_maintenance.csv`) includes various operational parameters, target labels indicating failure, and failure types. Key features include:

- `Air temperature [K]`
- `Process temperature [K]`
- `Rotational speed [rpm]`
- `Torque [Nm]`
- `Tool wear [min]`
- `Target` (0 for no failure, 1 for failure)
- `Failure Type`

### Methodology

1. **Data Exploration and Preprocessing**
   - Load the dataset and check for missing values.
   - Visualize the distributions of key features.
   - Normalize features using MinMaxScaler.
   - Split the data into training and testing sets with stratification.

2. **Model Training and Evaluation**
   - Train Decision Tree, Random Forest, and K-Nearest Neighbors classifiers.
   - Evaluate model performance using accuracy scores on both training and testing sets.

3. **Visualization**
   - Histograms and density plots for feature distributions.
   - Count plot for failure type distribution.

### Results

- **Decision Tree Classifier:**
  - Test Accuracy: 98%
  - Train Accuracy: 100%
  
- **Random Forest Classifier:**
  - Test Accuracy: 98.55%
  - Train Accuracy: 100%
  
- **K-Nearest Neighbors Classifier:**
  - Test Accuracy: 97.35%
  - Train Accuracy: 97.82%

The Random Forest classifier exhibited the highest accuracy, suggesting its effectiveness in predicting equipment failures.

### Conclusion

Machine learning models, particularly the Random Forest classifier, demonstrate significant potential in predicting equipment failures. By leveraging these models, predictive maintenance strategies can be optimized, reducing downtime and operational costs.

### Installation and Usage

1. **Clone the Repository**
   ```sh
   git clone https://github.com/madhu03111/Equipment_failure_detection.git
   cd equipment-failure-detection
   ```

2. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```

3. **Run the Analysis**
   Ensure the dataset (`predictive_maintenance.csv`) is in the same directory as the script.
   ```sh
   python equipment_failure_detection.py
   ```

4. **View Results**
   The script will print accuracy scores and display visualizations of the data and model performance.

### Dependencies

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn



