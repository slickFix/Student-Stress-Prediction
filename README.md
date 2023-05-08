# Student Stress Prediction Using Mobile Sensing Data
This is the final project report for ECE 284 Digital Health System. The aim of this project was to explore the possibility of predicting students’ stress conditions based on various remote sensed data along with Ecological Momentary Assessment (EMA) surveys sampled throughout the academic quarter.

# Dataset
The dataset used in this project is the StudentLife dataset, which consists of data from 48 Dartmouth students over a 10-week term to assess their mental health. The data includes physiological data collected from wearable devices and smartphones, as well as EMA surveys.

# Methodology
The project experimented with three different periods of aggregation windows (12 hours, 24 hours, and 48 hours) and various classifiers such as Logistic Regression, Random Forest, Support Vector Machines, and Light Gradient Boosting Machines. The Light Gradient Boosting Machine classifier achieved the highest AUC score of 0.76 for the 24-hour aggregation window for sensor data combined with EMA surveys.

# Results
The above modeling approach can be implemented through various mobile applications which can predict a student’s stress and suggest various intervention methods like meditation, exercise, etc.


* Table 1. AUC metric of different models using only sensing data

| Model                  | 12 Hour | 24 Hour | 48 Hour |
|------------------------|--------|---------|---------|
| LGBM                   | 0.67   | 0.70    | 0.72    |
| Logistic Regression | 0.65   | 0.71    | 0.70    |
| Support Vector Machines | 0.63  | 0.72    | 0.65    |
| Random Forest        | 0.70   | 0.65    | 0.72    |

* Table 2. AUC metric of different models using only sensing and EMA data

| Model                  | 12 Hour | 24 Hour | 48 Hour |
|------------------------|--------|---------|---------|
| LGBM                   | 0.70   | 0.76    | 0.75    |
| Logistic Regression | 0.69   | 0.71    | 0.70    |
| Support Vector Machines | 0.66  | 0.68    | 0.72    |
| Random Forest        | 0.71   | 0.72    | 0.73    |

# Conclusion
The project demonstrated the potential of utilizing mobile sensing data to predict a student’s stress level. The findings of this project can be used to develop mobile applications that can provide timely intervention and support to students experiencing high levels of stress.
