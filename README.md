# Project Logistic Regression Analysis of TCGA-COAD Clinical Data

# Author: Saranya Guvvala

# Date: 01-05-2024

# Programming Language & Version: Python 3.8

# Dependencies:
pandas
numpy
matplotlib
seaborn
scikit-learn

# Input:

clinical_data_ready_for_analysis.csv: Contains the clinical data for patients diagnosed with colorectal cancer, sourced from The Cancer Genome Atlas-Colon Adenocarcinoma (TCGA-COAD) dataset.
Script Description:
This Python script conducts a comprehensive analysis of clinical data from colorectal cancer patients to predict outcomes using logistic regression. The script first performs an exploratory data analysis (EDA) to understand the distribution and relationships of various clinical variables. Following EDA, logistic regression is applied with class weight adjustments to handle potential imbalances in the dataset. Key performance metrics are evaluated at different decision thresholds to optimize the model's predictive accuracy.

# Model Building:

The dataset is split into training (70%) and testing (30%) sets to evaluate the model's performance.
Logistic regression is used with adjusted class weights to fairly represent both outcome classes in the model training process.
The model's performance is initially tested at a default threshold of 0.5 and further evaluated at an adjusted threshold of 0.6 to refine prediction accuracy.

# Output Files:

model_performance_metrics.txt: Contains the confusion matrix and classification reports at both tested thresholds.
ROC_curve.png: A plot of the Receiver Operating Characteristic curve, illustrating the model's ability to discriminate between patient outcomes.

# Further Analysis:
Upon completion of the logistic regression analysis, further studies could involve:

Integrating genomic data with clinical variables to enhance the model's prognostic capabilities.
Cross-validation studies to verify the model's robustness and reliability across different patient subsets.
Usage Instructions:

Ensure all dependencies are installed using pip install -r requirements.txt.
Run the script using the command python logistic_regression_analysis.py.
Review the output files for detailed performance metrics and visualizations of the model's efficacy.
