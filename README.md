# Data Classification via an Improved Supervised Learning Algorithm

## Project Objective 
Develop and investigate an algorithm for data classification to improve: (I) the accuracy of widely used classification algorithms such as K-Nearest Neighbours (KNN), Support Vector Machines (SVM), Naive Bayes (NB), and Logistic Regression (LR) for recall-oriented Machine Learning (ML) tasks such as disease diagnosis, and (II) the speed of the existing MAX FS classification methods while improving/preserving the accuracy.

## Challenges 
The literature MAX FS algorithms are already known to provide high performance for binary classification. However, the state-of-the-art MAX FS algorithms have rarely been used and investigated since they are slow. Therefore, the main requirement is to increase their speed without loss of accuracy.

## Achievements
According to the experimental results, the introduced classification algorithm

- Provides better total accuracy compared to KNN, SVM, NB, and LR methods with and without hyperparameter tuning. 
- Improves the speed of the literature MAX FS classification methods by about 94% while improving the accuracy.
- Provides promising results for recall-oriented machine learning tasks such as disease diagnosis. 

## Related Pulications
### Refereed Journal Publication

##### •	F. F. Firouzeh, J. W. Chinneck, S. Rajan, "Faster Maximum Feasible Subsystem Solutions for Dense Constraint Matrices,” Submitted to Computers and Operations Research Journal.

### Refereed Conference Publications

##### •	F. F. Firouzeh, J. W. Chinneck, S. Rajan, "A Faster MAXimum Feasible Subsystem Algorithm for Binary Classification," Accepted in 2021 IEEE International Symposium on Medical Measurements and Applications (MeMeA).



-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###### Some details of the experimental setup are summarised in below. For more detail refer to the papers metioned above.

### Datasets
 Binary classification problems derived from datasets in the UCI Repository of Machine Learning Databases https://archive.ics.uci.edu/ml/datasets.php. The following tables summarize the characteristics of the datasets used in two set of experiments (Scenario I and Scenario II). In the first scenario, the training set is identical to the entire dataset to compare with previous results of Chinneck's paper (https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632 ). In Scenario II, real-world medical and biological datasets selected for the experiments. The task is to predict whether the patient has the disease (Class 1) or not (Class 0). 10-fold cross validation used to prevent over fitting and better generalization. The same folds used throughout the implementation for all the models to ensure uniformity.

![ClassificationData](https://user-images.githubusercontent.com/59096353/114231621-a9c6b880-9948-11eb-9bc4-508e4ba45e78.png)

### Hyperparameter Tuning

Hyperparameter tuning is required to obtain best performance for some classifiers. For the methods that require hyperparameter tuning, two sets of results are reported: (1) default settings without hyperparameter tuning "Def", and (2) with hyperparameter tuning "Tune" ("Def" applies if unspecified). A recent study (Bahel et al. paper https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632), is considered here to select hyperparameter optimization methods and search ranges.

### Tools/Software
Python (Scikit-learn, Pandas, Seaborn, Matplotlib, and Plotly), MATLAB, MOSEK, LaTeX.
