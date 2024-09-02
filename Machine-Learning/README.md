# Machine Learning for Nitrogen Removal in Constructed Wetlands under Antibiotics Stress

This Github includes codes and data for the project of 'Machine Learning for Nitrogen Removal in Constructed Wetlands under Antibiotics Stress'.

# Authors
Jianghui Feng 1#, Zhikun Zou 2#, Zhiyong Zhang 3*, Lei Chen 1, Ming-Lai Fu 4, Haiyan Li 2, Baoling Yuan 1*

School of Municipal Engineering Environmental Engineering Resources and Environment
Key Laboratory of Water Environment in Songliao Basin, Jilin Jianzhu University, No.5088 Xincheng Street, Nanguan District, Changchun City, Jilin Province 130119, China

# Abstract 
Microbial synergies and factors for designing constructed wetlands have been limited in traditional research, while it will be overcome using machine learning analysis. Herein, the different machine learning, include GPR, GA-SVM, RF, and XGBoost, were applied to investigate the degradation of TN and antibiotics by constructed wetland. In addition, the contributions of each feature were explained by the importance analysis, and the contribution of input features to TN and antibiotics removal were quantified using mean absolute shapley (MAS) methods. The results showed that influent water quality had the greatest effect on TN removal (52.4%) in constructed wetlands under antibiotic stress. An immutable parameter, volume of constructed wetland, the effect on TN removal (10.6%) was much greater than that on antibiotic removal (0.7%), indicating the volume should be expanded to meet the requirement of TN removal in the design of constructed wetland. Besides an adaptive constructed wetland system would be established by adjusting the inlet water quality and adding specific microorganisms for conducive to the collaborative TN removal and organic pollutants by constructed wetlands. This study reveals nitrogen removal in constructed wetlands under antibiotics stress and provides directions to guide the design and operation of constructed wetlands under the stress of organic pollutants.

# Description
DATA_2.csv - raw data of ( 'Time', 'Deep', 'Length', 'HRT', 'COD', 'TN', 'NH4-N', 'C/N', 'c(A)', 'CSC', 'XLogP3', 'WI', 'RA(P)', 'RA(F)', 'RA(B)', 'RA(A)' ) .


Pearson_correlation.ipynb - Draw a correlation heat map.

GPR.ipynb - Establish Gaussian process regression to predict the removal rate code.

ga-svm.ipynb - Constructing genetic algorithm - Support vector machine regression prediction of removal rate.

XGBoost.ipynb - Code that builds extreme gradient lift to predict removal rates.

RF.ipynb - Code for building random forest prediction removal rates.

Feature_importance_analysis.ipynb - Code for a feature importance analysis tool (FSW, Shapley method, and PFI) based on XGB, GPR, GA-SVM, and RF results.

Models- This folder includes training models for rf (RF.PKL), XGB (xgbr.pkl), GPR (GPR.PKL) and GA-SVM (GA_SVM.pkl).