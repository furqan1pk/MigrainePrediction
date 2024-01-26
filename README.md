# Personalized Migraine Risk Assessment and Attack Prediction
## Key Technologies and Tools

![Python](https://img.shields.io/badge/Python-3.8-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.2.4-blue)
![NumPy](https://img.shields.io/badge/NumPy-1.19.5-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.3.4-blue)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11.1-blue)
![LSTM](https://img.shields.io/badge/LSTM-Networks-blue)

- **Programming Language**: Python
- **Major Libraries**: Pandas, NumPy, Matplotlib, Seaborn, cvxEDA
- **Machine Learning Algorithms**: LSTM Networks, RNN
- **Keywords**: Time-series Analysis, Sensor Data Processing, Environmental Data Analysis, Stress Level Analysis, Migraine Prediction, Data Preprocessing and Cleaning

## Introduction
This repository hosts a Python-based project aimed at leveraging multi-modal data for personalized migraine risk assessment and attack prediction. It encompasses data preprocessing, visualization, and the implementation of advanced machine learning models, including Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM) networks.

## Key Components

### Data Collection
Data is collected using Empatica E4 wearable sensors, capturing physiological parameters like heart rate, electrodermal activity (EDA), blood volume pulse, and XYZ raw acceleration. Additionally, sleep quality, duration, triggers, and medications are tracked daily. Environmental data, including humidity, pressure, temperature, and UV index, are gathered via the Dark Sky API.

### Data Preprocessing
We apply advanced techniques to preprocess the time-series data, involving noise removal and normalization. Tools like cvxEDA are utilized for decomposing EDA signals into phasic and tonic components, offering crucial insights into stress levels.

### Data Visualization
Our approach includes sophisticated data visualization methods. We plot time-series data across a 24-hour scale, integrating various parameters and showcasing correlations, sleep patterns, and migraine severity.

### Data Analysis
We conduct comprehensive analyses, including input and output correlations, statistical analysis of stress peaks, and migraine episode occurrence. This includes exploring correlations between environmental factors like wind gusts and physiological responses.

### Machine Learning and Predictive Modeling
The core of our project involves using Long Short-Term Memory (LSTM) networks for predictive modeling. We train our models on segmented data to predict future migraine episodes, both for individual patients and across different patients. The project also delves into classification and clustering techniques, offering detailed insights into migraine patterns.

## Repository Structure

- **01_Preprocessing_Data.ipynb**: Initial preprocessing of the dataset, preparing it for machine learning analysis.
- **01b_Additional_Data_Cleaning.ipynb**: Supplementary data cleaning processes, enhancing the quality of the dataset.
- **02a_Sensor_Data_Visualization.ipynb** and **02b_Sensor_Data_Visualization_Extended.ipynb**: Visualization of patient sensor data, providing insights into the dataset characteristics.
- **03_Migraine_Prediction_Models.ipynb**: Implementation and evaluation of RNN and LSTM models for predicting migraine episodes.
- **04_Data_Plots_Matplotlib.ipynb** and **05_Data_Plots_Pandas.ipynb**: Additional data plotting and visualization using Matplotlib and Pandas.
- **06_Weather_Data_Extraction.ipynb**: Extraction and preprocessing of weather data relevant to migraine prediction.
- **07_Comprehensive_Analysis.ipynb**: The comprehensive and final analysis, combining all aspects of the dataset and modeling.
- **08_PT_Diary_Data_Analysis.ipynb** and **09_CSV_Data_Analysis_and_Plotting.ipynb**: Analysis of patient diary data and CSV file processing.
- **Migraine_Prediction_Study_Report.docx**: Detailed documentation of the machine learning process and the insights derived from the study.

## Setup and Installation

Ensure Python is installed on your system. Install necessary libraries using the following command:

```bash
pip install -r requirements.txt
