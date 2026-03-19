# S.M.A.R.T. Hard Drive Failure Prediction

## Overview
This project applies Machine Learning to predict hard drive failures using S.M.A.R.T. (Self-Monitoring, Analysis, and Reporting Technology) sensor data. By analyzing operational metrics from the last quarter of 2025, the model identifies patterns that precede physical drive failures, allowing for proactive maintenance in data centers.

## Team Members
* **Bevnoty Mamdouh** (Leader) - 
* **Andrew Ashraf** - 
* **Amr Danny** - 
* **Mohamed Samaha** - 
* **Mohamed Mostafa** - 

## Project Pipeline
1. **Data Wrangling:** Processed 92 daily files containing hundreds of thousands of drive records. Extracted all failed drives and sampled 0.5% of healthy drives to balance the dataset and prevent memory crashes.
2. **Dimensionality Reduction:** Cleaned metadata, handled missing values, and used SelectKBest (ANOVA F-value) to isolate the top 10 most critical physical sensors.
3. **Model Training & Evaluation:** Trained and compared three algorithms:
   * Logistic Regression (Baseline)
   * Decision Tree
   * **Random Forest (Champion):** Achieved the best performance, catching the highest percentage of actual drive failures while significantly minimizing false positive "alarms."

## Tech Stack
* **Language:** Python
* **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn

## Setup & Execution
*(Note: Raw data files are excluded from this repository due to their massive size. To run this locally, you must provide the `data_Q4_2025` folder).*

1. Clone the repository:
   ```bash
   git clone [https://github.com/bmbbggp/smart-sensor-pattern-project.git](https://github.com/bmbbggp/smart-sensor-pattern-project.git)