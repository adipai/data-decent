# Data decent
Automated Software Engineering (Group 1) research project where we :
* Create an intelligent data pruning mechanism
* Perform statistical analysis of intelligently choosing 'least' amount of 'best' data  for data mining tasks

## Datasets
- Breast Cancer (classification)
- Churn (classification)
- JS_Vuln (classification) A
- Ambari_Vuln (classification) A
- Defect_Eclipse_JDT_Core (classification) R
- Defect_Eclipse_PDE_UI (classification) R
- Moodle_Vuln (classification) D
- Defect_Mylyn (classification) D

## Data sampling techniques used/created
### Baselines
- Random Pruning (under-sampling)
- Random Oversampling (over-sampling)
- SMOTE (over-sampling)
- SVM SMOTE (over-sampling)
- Gaussian Copula-SDV (over-sampling)
- Recursive Random Projections-RRP (over-sampling)
### Proposed + devised technique 
- Intelligent Pruning (under-sampling)
  
## Learners used to test sampling techniques
- Logistic Regression
- SVM
- Decision Tree

## Results
To see scott-knott plots, go to results/{dataset_name}/sk/

## Citations
* X. Ling, T. Menzies, C. Hazard, J. Shu and J. Beel, "Trading Off Scalability, Privacy, and Performance in Data Synthesis," in IEEE Access, vol. 12, pp. 26642-26654, 2024, doi: 10.1109/ACCESS.2024.3366556.
keywords: {Synthetic data;Clustering algorithms;Data models;Engines;Biomedical imaging;Generative adversarial networks;Data privacy;Regression analysis;Classification algorithms;Scalability;Homomorphic encryption;Synthetic data generation;privacy preservation;regression;classification},
* https://github.com/yrahul3910/SyntheticOversampling {RRP oversampling}

