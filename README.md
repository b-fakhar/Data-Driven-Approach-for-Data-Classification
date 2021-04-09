# Novel Data Mining Algorithm for Classification

### Objective 
Develope and investigate a new data mining algorithm to solve classifictaion problems. The new classification algorithm is developed to improve: (1) the recall score of the well-known classification algorithms such as K-Nearest Neighbours (KNN), Support Vector Machines (SVM), Naive Bayes (NB), and Logistic Regression (LR) for recall-oriented Machine Learning (ML) tasks such as disease diagnosis, and (2) improve the speed of the existing MAX FS classification methods while improving or preserving the accuracy.

### Challenges 


### Achivements
According to the experimental results, the introduced classification algorithm

- Provides better total accuracy compared to KNN, SVM, NB, and LR methods with and without hyperparameter tuning. 
- Improves the speed of the lterature MAX FS classification methods by about 94% while improving the accuracy.
- Provides promising results for recall-oriented machine learning tasks such as disease diagnosis. 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### The following sections detail the experimental setup

### Datasets
 Binary classification problems are derived from datasets in the UCI Repository of Machine Learning Databases https://archive.ics.uci.edu/ml/datasets.php. The following tables  summarize the characteristics of the datasets used in two set of experiments (Scenario I and Scenario II). In the first scenario, the training set is identical to the entire dataset to compare with previous results of Chinneck's paper (https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632 ). In Scenario II, real-world medical and biological datasets for disease diagnosis are used. The task is to predict whether the patient has the disease (Class 1) or not (Class 0). The same folds are used throughout the implementation for all the models to ensure uniformity.

![ClassificationData](https://user-images.githubusercontent.com/59096353/114231621-a9c6b880-9948-11eb-9bc4-508e4ba45e78.png)

### Hyperparameter Tuning

Hyperparameter tuning is required to obtain best performance for some classifiers. For the methods that require hyperparameter tuning, two sets of results are reported: (1) default settings without hyperparameter tuning "Def", and (2) with hyperparameter tuning "Tune" ("Def" applies if unspecified). A recent study titled " comparative study on various binaryclassification algorithms and their improved variant for optimal performance", provides a comprehensive overview of hyperparameter optimization of common ML models. 

In experiments, the experimental results of the comparators are reported with and without hyperparameter tuning. Hyperparameters are tuned using the hyperparameter optimization methods and search ranges suggested in the above mentioned paper. There is no need to tune hyperparameters in NB and LR since the performance of these models mainly depends on how well the datasets follow the Gaussian distribution and normal distribution, respectively. Table \ref{parTUN} summarizes the hyperparameters ``HP", selected hyperparameter optimization methods ``HPO", and search range for the KNN and SVM classifiers.





