
# Overview
This project aims to conduct an in-depth analysis of credit card fraud detection using a data-driven approach. A key focus of the study is the evaluation of various machine learning models, with particular emphasis on optimizing recall to capture a higher number of fraud cases while maintaining an acceptable level of precision. This comprehensive approach not only aims to improve fraud detection accuracy but also contributes to the broader understanding of effective strategies in combating financial fraud in real-world scenarios.

**Data Link:** https://www.kaggle.com/datasets/kartik2112/fraud-detection

# Repository Contents
- `notebooks/Fraud.ipynb`: A Jupyter notebook containing the code, analysis, and machine learning model implementations for the project. This notebook includes data preprocessing, exploratory data analysis, feature engineering, class balancing, model training, and evaluation sections.
- `docs/results.xlsx`:  An Excel file containing the results of various models tuned with specific parameters. Each sheet within the file corresponds to a different model, providing a comprehensive overview of the model performance.
- `docs/CreditCard_Fraud_Detection.pdf`: A presentation detailing the project's objectives, methodology, analysis, findings, and conclusions. This presentation is designed to provide a clear and concise overview of the project for stakeholders.

# Methodology
1. **Data Collection**
   - Sourced from Kaggle; covers transactions from 1000 customers and 800 businesses between January 2019 and December 2020.

2. **Data Preprocessing**
   - Cleaned to remove missing values and duplicates.
   - Engineered features like transaction distances, time-related attributes, and simplified analysis by segmenting states into regions (Northeast, Midwest, South, West) and consolidated numerous job titles into broader categories.
     
3. **Feature Selection and Normalization**
   - Excluded non-predictive information and normalized numerical features to ensure model compatibility and effectiveness.

4. **Dataset Balancing**
   - Employed Random Under Sampling to address class imbalance in the large dataset, creating a balanced distribution for the modeling process.

5. **Modeling and Evaluation**
   - Tested various models (e.g., Logistic Regression, KNN, Decision Trees, Random Forest, Gradient Boosting, Multi-Layer Perceptron), emphasizing recall to optimally detect fraud.
   - Evaluated models based on precision, recall, F1-score, and accuracy.

6. **Feature Importance**
   - Conducted post-modeling analysis to identify and interpret the most influential features in fraud prediction, highlighting the significance of transaction amount, transaction time, and specific categories like high-value internet and POS transactions.

# Installation and Usage
To set up the project, clone the repository, install dependencies, and navigate to the directory. Run Jupyter Notebook to view the project:
```bash
git clone https://github.com/Shanmukhi1920/Fraud_Detection
cd Fraud_Detection
pip install -r requirements.txt
jupyter notebook
```
Then, open `Fraud.ipynb` in Jupyter in the `notebooks/` directory.

# Key Findings
**Model Performance:** Random Forest outperformed other models in terms of recall, with Gradient Boosting showing similar overall effectiveness.

**Feature Importance:** High-value internet and Point Of Sale (POS) transactions were key indicators of fraud. Other notable features include transaction amount, hour, and gas/transport categories.





