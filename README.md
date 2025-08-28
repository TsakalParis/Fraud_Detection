# Credit Card Fraud Detection
A comprehensive machine learning project for detecting fraudulent credit card transactions using various algorithms and ensemble techniques.

Project Overview
This project implements and compares multiple machine learning models for credit card fraud detection, including:

Tree-based models: XGBoost, CatBoost, Random Forest

Anomaly detection: Isolation Forest with various contamination parameters

Ensemble methods: Simple averaging, stacking, SHAP-weighted ensembles, and SHAP-guided stacking

Feature analysis: SHAP-based feature importance and dependence plots

Dataset
The project uses the Credit Card Fraud Detection dataset from Kaggle, which contains transactions made by European cardholders in September 2013. The dataset is highly imbalanced, with only 492 frauds out of 284,807 transactions.

Key Features
Data Preprocessing: Standard scaling of transaction amounts while preserving the original distribution of PCA-transformed features (V1-V28)

Multiple Modeling Approaches:

Variotional Auto Encoders for detecting fraudulent transactions via reconstruction error.

Supervised learning with tree-based models

Unsupervised anomaly detection

Advanced ensemble techniques

Feature Selection: Custom feature sets for different models based on SHAP analysis

Performance Evaluation: Comprehensive metrics including ROC AUC, PR AUC, F1-score, precision, and recall

Explainability: SHAP analysis for model interpretability and feature importance

Installation
bash
# Clone the repository
git clone https://github.com/your-username/credit-card-fraud-detection.git
cd credit-card-fraud-detection

# Install dependencies
pip install -r requirements.txt
Usage
The project is organized in a Jupyter notebook that can be executed step-by-step:

Data loading and preprocessing

Model training and evaluation

Ensemble method implementation

Results visualization and comparison

Results
The project compares various models and ensemble techniques, with the best performing methods achieving:

High ROC AUC scores (>0.98)

Excellent precision-recall balance

Effective fraud detection with minimal false positives

Methodology
Data Preparation: Stratified train-test split with standardized amount scaling

Model Training: Multiple algorithms with hyperparameter tuning

Ensemble Construction: Various ensemble strategies to combine model strengths

Evaluation: Comprehensive metrics and visualizations for performance comparison

Interpretation: SHAP analysis for understanding model decisions

File Structure
text
credit-card-fraud-detection/
├── credit_card_fraud_detection.ipynb  # Main notebook
├── requirements.txt                    # Dependencies
└── README.md                          # Project documentation

Technologies Used
Python, Scikit-learn, XGBoost, CatBoost, SHAP, Matplotlib/Seaborn, Pandas/Numpy

License
This project is licensed under the MIT License - see the LICENSE file for details.
