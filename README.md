# Data Driven Approach for Data Classification

# Summary
- Developed a novel data-driven approach to enhance the speed of a supervised method while maintaining high classification accuracy, resulting in a significant improvement in computational efficiency.
- Implemented an end-to-end machine learning pipeline for the classification of biological datasets from the UCI repository, leveraging tools such as Matplotlib and Seaborn to visualize the data and gain valuable insights.
- Conducted data preparation tasks, including handling outliers, missing values, and imbalanced data, to ensure the accuracy and reliability of the ML models.
- Evaluated multiple ML models using cross-validation, both with and without hyperparameter tuning, to identify the most effective approach for the given data.
- Demonstrated the superiority of the proposed data-driven approach, which on average improves the speed of existing supervised methods by 80%, while achieving better performance than popular classification algorithms such as k-NN, Logistic Regression, Naïve Bayes, and SVM for biological data.

# Skills/Tools
- Machine Learning, Optimization, Feature Engineering, Hyperparameter Tuning, Python (Scikit-learn, Pandas, numpy, Seaborn, Matplotlib), MATLAB, MOSEK, LaTeX. 

# Related Pulications
### Refereed Journal Publication

##### •	F. F. Firouzeh, J. W. Chinneck, S. Rajan, "Faster Maximum Feasible Subsystem Solutions for Dense Constraint Matrices,” Submitted to Computers and Operations Research Journal.

### Refereed Conference Publications

##### •	F. F. Firouzeh, J. W. Chinneck, S. Rajan, "A Faster MAXimum Feasible Subsystem Algorithm for Binary Classification," Accepted in 2021 IEEE International Symposium on Medical Measurements and Applications (MeMeA).
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
##### Some information about the developed algorithm, datasets, and experimental results are summarised in below. For more details, please refer to the mentioned papers.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Developed Algorithms
The developed Algorithm, Algorithm 2E1, is based on the following observation:
![image](https://user-images.githubusercontent.com/59096353/128287407-d512a278-0217-4d89-a680-bb9a7260f6f2.png)

The steps of the developed classification method is explained in the following flowchart and pseudocode.
<!-- ![image](https://user-images.githubusercontent.com/59096353/128286907-5d123cb3-f6b4-418a-b6f8-ca7e9c1cf53a.png)
![image](https://user-images.githubusercontent.com/59096353/128287248-f38b4621-1b57-4296-a9a0-ef061faf1205.png) -->
![image](https://user-images.githubusercontent.com/59096353/128288123-323e6f79-847a-49f9-96b6-0b37b57587bd.png)



### Datasets
 Binary classification problems derived from datasets in the UCI Repository of Machine Learning Databases https://archive.ics.uci.edu/ml/datasets.php. The following tables summarize the characteristics of the datasets used in two set of experiments (Scenario I and Scenario II). In the first scenario, the training set is identical to the entire dataset to compare with previous results of Chinneck's paper (https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632 ). In Scenario II, real-world medical and biological datasets selected for the experiments. The task is to predict whether the patient has the disease (Class 1) or not (Class 0). 10-fold cross validation used to prevent over fitting and better generalization. The same folds used throughout the implementation for all the models to ensure uniformity.

![ClassificationData](https://user-images.githubusercontent.com/59096353/114231621-a9c6b880-9948-11eb-9bc4-508e4ba45e78.png)

### Comparators
- Original Algorithm 2(∞) and original Algorithm 2(1).
- K-Nearest-Neighbour (KNN),  Logistic Regression (LR), Gaussian Naïve Bayes (NB), Support Vector Machine (SVM).

### Hyperparameter Tuning

Hyperparameter tuning is required to obtain best performance for some classifiers. For the methods that require hyperparameter tuning, two sets of results are reported: (1) default settings without hyperparameter tuning "Def", and (2) with hyperparameter tuning "Tune" ("Def" applies if unspecified). A recent study (Bahel et al. paper https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632), is considered here to select hyperparameter optimization methods and search ranges.

# Summary of Experimental Results
![image](https://user-images.githubusercontent.com/59096353/128287835-47823433-3d9e-4cca-b426-5e9e733fcd48.png)
