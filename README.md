# SQL-Injection-Detection

## Overview
SQL Injection Detection is a cybersecurity-focused project that aims to develop an efficient algorithm to detect malicious SQL injection attacks. This project utilizes a dataset of network traffic, processed through supervised learning algorithms, to classify SQL injection threats and enhance system security.

## Objective
1. **Enhance Cybersecurity:** Protect sensitive information stored and transmitted online.
2. **Detect Malicious IPs:** Identify IP addresses associated with SQL injection attacks.
3. **Focus on Attack Types:** Target Union Query and Blind Query-based SQL injection types.
4. **Evaluate Algorithms:** Develop and test classification models to achieve accurate predictions.

## Dataset
The dataset used in this project is composed of malicious and benign network traffic:
- **Source:** Collected using the DOROTHEA framework.
- **Format:** Numeric features with binary categorical labels.
- **Split:** Two datasets—D1 for training and D2 for testing.
- **Protocol:** Follows NetFlow V5 standards.
- **Dataset Links:**
  - [Training Dataset (D1)](https://drive.google.com/file/d/1EGOgQ1vP1Bf4tc6q2V5uffrW2NyzsuA8/view?usp=drive_link)
  - [Testing Dataset (D2)](https://drive.google.com/file/d/1EMI1nWXmKCVSu8VFRIiQ7seoPb0Rv447/view?usp=drive_link)

## Algorithms and Methodology
1. **Exploratory Data Analysis (EDA):**
   - Feature importance analysis to identify key predictors.
   - Standardized numerical features and encoded categorical variables.
2. **Model Selection:**
   - **Logistic Regression with L1 Regularization:** For interpretable, linear relationships.
   - **Random Forest:** To handle non-linear relationships and complex decision boundaries.
   - **XGBoost:** To optimize model accuracy and handle imbalanced classes.
3. **Evaluation Metrics:**
   - C-statistics
   - Accuracy score
4. **Feature Engineering:**
   - Selected the top 15 features to reduce dimensionality and overfitting.
   - Data preparation included normalization and handling missing values.

## Results
- The models successfully classified benign and malicious network traffic.
- Visualizations (scatter plots, histograms, bar charts) illustrated relationships between features and SQL injection labels, validating the effectiveness of feature engineering and preprocessing.

## Challenges and Future Work
- **Challenges:**
  - Dataset size limited the use of deep learning models due to potential overfitting.
  - Lack of timestamp attributes affected the ability to detect attack sequences.
- **Future Directions:**
  - Incorporate timestamp and geospatial attributes to enhance classification accuracy.
  - Explore deep learning models (CNN, RNN) for larger datasets.


