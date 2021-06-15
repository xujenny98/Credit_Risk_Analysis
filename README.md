# Supervised machine learning and credit risk
# Overview of the loan prediction risk analysis:
Machine Learning Models are evaluated against financial data to determine credit risk. This is performed within Python & Jupyter Notebook in Anaconda.
Key resources utilized are:
-sklearn
-imbalanced learn

Goal is to compare 6 Machine Learning Models against the raw data set & provide judgement on the models based on observations for Accuracy, Precision, Recall:

-Naive Random Oversampling
-SMOTE Oversampling
-Undersampling
-Combination (Over and Under) Sampling
-Balanced Random Forest Classifier
-Easy Ensemble AdaBoost Classifier

# Results:
# Naive Random Oversampling
![naive_oversampling](https://user-images.githubusercontent.com/77771292/122001944-1b731680-cd7f-11eb-9c85-2676693758c6.PNG)
# SMOTE Oversampling 
![smote_oversampling](https://user-images.githubusercontent.com/77771292/122002028-3b0a3f00-cd7f-11eb-97bb-556901af1dce.PNG)
# Clustered Centroids Undersampling 
![clustered_centroids_undersampling](https://user-images.githubusercontent.com/77771292/122002114-54ab8680-cd7f-11eb-8596-b8e48eb61b12.PNG)
# Combination (Over and Under) Sampling with SMOTEENN 
![smoteenn_over_and_undersampling](https://user-images.githubusercontent.com/77771292/122002249-80c70780-cd7f-11eb-97c6-cf4471ac2151.PNG)
# Balanced Random Forest Classifier 
![balanced_random_forest](https://user-images.githubusercontent.com/77771292/122002338-9d633f80-cd7f-11eb-9260-15a7de4c1745.PNG)
# Easy Ensemble AdaBoost Classifier 
![easy_ensemble_classifier](https://user-images.githubusercontent.com/77771292/122002410-b10ea600-cd7f-11eb-94b9-68958bb4126e.PNG)

# Summary:
Best overall model to use is "Easy Ensemble AdaBoost Classifier" based on higher Balanced Accuracy & Sensitivity result.
Precision had no factor in decision since all models were essentially equivalent.

F-score should also be considered when evaluating the models.
Although not requested as focus as part of the challenge, review of F-Score finds:

Naive Random Oversampling = 0.75
SMOTE Oversampling = 0.81
Undersampling = 0.58
Combination (Over and Under) Sampling = 0.72
Balanced Random Forest Classifier = 1.00
Easy Ensemble AdaBoost Classifier = 1.00
Of interest here is that Random Forest & Adaboost both have same F-Score (1.00), but Balanced Accuracy is less for Random Forest vs AdaBoost (0.6830 < 0.7325).
This reinforces a need to look at overall results in detail versus determination through single score selection.
