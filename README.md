# Data decent
Automated Software Engineering (Group 1) research project where we :
* Create an intelligent data pruning mechanism
* Perform statistical analysis of intelligently choosing 'least' amount of 'best' data  for data mining tasks

## Abstract
Data quality is a critical metric in ensuring that machine learning models perform well on real-world tasks. More specifically, in the case of class-imbalanced datasets, sampling strategies play an important role in deciding the quality of data fed to machine learning models. Our study introduces a novel approach to data under-sampling called 'intelligent data pruning,' which employs advanced clustering techniques to identify and eliminate redundant or irrelevant data points. By significantly reducing dataset size without loss of 'informative' data samples, our method optimizes the model training process for low computational resource utilization while enhancing model generalization. We extensively compare our method with existing under-sampling and over-sampling techniques on various software engineering datasets using three different learners: Logistic Regression, Decision Tree, and Support Vector Machine. Traditional data sampling methods like random sampling, SMOTE as well as sophisticated techniques such as Gaussian Copula and Recursive Random Projection based oversampling techniques are included in our evaluation as benchmarks. Through rigorous experimentation and performance analysis, we demonstrate the superior accuracy of our proposed data pruning method across diverse datasets and learners. Additionally, we provide insights into the underlying mechanisms driving its effectiveness and its potential applications in real-world scenarios with large-scale datasets and computational constraints. 

## Datasets
- Breast Cancer (classification)
- Churn (classification)
- JS_Vuln (classification)
- Ambari_Vuln (classification)
- Defect_Eclipse_JDT_Core (classification)
- Defect_Eclipse_PDE_UI (classification)
- Moodle_Vuln (classification)
- Defect_Mylyn (classification)

## Data sampling techniques used/created
### Baselines
| Technique                          | Type            |
|------------------------------------|-----------------|
| Random Pruning    | Under-sampling  |
| Random Oversampling | Over-sampling   |
| SMOTE               | Over-sampling   |
| SVM SMOTE           | Over-sampling   |
| Gaussian Copula-SDV | Over-sampling   |
| Recursive Random Projections-RRP | Over-sampling|

### Proposed + devised technique 
| Technique                      | Type           |
|--------------------------------|----------------|
| Intelligent Data Pruning  | Under-sampling |

  
## Learners used to test sampling techniques
- Logistic Regression
- SVM
- Decision Tree

## How to run code
The code (notebooks) used has been provided under `/src`. For experimentation, notebooks under `src/experiments` showcase how to load the data and run for an interation. For running experiments in the larger context notebooks under `/src/automation` specifiy the details of all the experiments runs and is also the main source of data collected.

`/src/analyse_scott_knott.ipynb` - This notebook takes the results from the previous steps and plots the scott knott graphs. These graphs are stored under `/results/**/sk/` respectively for all the datasets.

``

## Results
Find scott-knott plots, go to results/{dataset_name}/sk/

### Radar plot of results
![radar_chart](https://github.com/adipai/data-decent/assets/22258487/1446cad5-3fba-4263-94d2-5ad015bdb1d9)

As we can see, the area covered by Intelligent Data Pruning(orange line)  is much higher than other techniques.

## Citations
* X. Ling, T. Menzies, C. Hazard, J. Shu and J. Beel, "Trading Off Scalability, Privacy, and Performance in Data Synthesis," in IEEE Access, vol. 12, pp. 26642-26654, 2024, doi: 10.1109/ACCESS.2024.3366556.
keywords: {Synthetic data;Clustering algorithms;Data models;Engines;Biomedical imaging;Generative adversarial networks;Data privacy;Regression analysis;Classification algorithms;Scalability;Homomorphic encryption;Synthetic data generation;privacy preservation;regression;classification},
* https://github.com/yrahul3910/SyntheticOversampling {RRP oversampling}

## Team members
[Rishi Singhal](https://www.linkedin.com/in/rishi-singhal1101/)<br/>
[Deepak Rajendran](https://www.linkedin.com/in/deepr41)<br/>
[Aditya Pai Brahmavar](https://www.linkedin.com/in/adityapai16/)<br/>
