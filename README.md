
# Drug Efficacy Recommendation and Repurposing System for Glioblastoma Using Machine Learning


This repository contains the implementation of a machine learning pipeline for  Drug Efficacy Recommendation and Repurposing System for Glioblastoma Using Machine Learning. 

## Overview

The notebook demonstrates the following steps:
1. Importing necessary libraries
2. Loading and preparing the data
3. Feature engineering
4. Data preparation for machine learning
5. Model training and evaluation
6. Drug screening and repurposing experiments

## Dependencies

Ensure you have the following libraries installed:
- pandas
- numpy
- matplotlib
- scikit-learn
- pycaret


## Data

1. Input Data
2. panCancer_train_CGC_657_DR_Drug_features_new_df.csv: 
3. Training data for pan-cancer
4. GBM_train_CGC_657_DR_Drug_features_new_df.csv: 
5. Training data for GBM
6. featureScore.csv: 
## Supplementary 
1. feature score data
2. diseaseNames.csv: List of disease names
3. 657_Gene_name.csv: List of gene names
4. moleculeNames_v1.csv: List of molecule names
## Output Data
The output data and models are saved in the result and models directories, respectively:

- LabelModel10fold.csv
- feature.csv
- LGBM10fold.csv
- unseen_predict.csv
- GBM_Carmustine_pred.csv
- GBM_Temozolomide_pred.csv
- Final_et_LNIC50_Model_25June2022
- Final_lgbm_Model_25June2022
## Steps
1. Importing Libraries
Necessary libraries are imported for data manipulation, visualization, and machine learning.

2. Load Data
Training datasets are loaded and concatenated for pan-cancer analysis.

3. Feature Engineering
Features with a score less than 70 are removed, and the relevant features are selected for analysis.

4. Data Preparation for ML Operation
Datasets are prepared for drug repurposing and screening experiments. Specific drug data is extracted for testing, and the remaining data is split into training and test sets.

5. Quantile Transformation of Target
Quantile transformation is applied to the target variable (LN_IC50) to handle skewness.

6. Model Selection for Quantile Inverse Transformation
The PyCaret environment is set up, and a Light Gradient Boosting Machine (LightGBM) model is trained to learn the relationship between transformed and original target variables. The model is saved for future use.

7. Drug Screening Model Development
The PyCaret environment is set up for the main dataset, and various regression models are trained. The best-performing model is saved.

8. Drug Screening Experiment with Test Data
Predictions are made on the test data using the trained model, and the results are saved.

9. Drug Repurposing Experiment
The trained model is used to predict drug resistance for specific GBM drugs, and the results are saved.

## Usage
-Ensure all dependencies are installed.
-Place the input data files in the correct directories as indicated.
-Run the notebook cells sequentially.
-Results and trained models will be saved in the specified directories.
## Conclusion
-This notebook provides a comprehensive pipeline for rug Efficacy Recommendation and Repurposing System for Glioblastoma Using Machine Learning. The use of quantile transformation, feature engineering, and robust model evaluation ensures high-quality predictions that can aid in personalized medicine and pharmacogenomics research.

## Contact Information
For any questions or issues, please contact [xajidnaveed@gmail.com].
