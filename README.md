# The Smith Parasite: Machine Learning Course Project - MDSAA-DS - Fall 2022


# Introduction


A newly discovered disease, identified as the Smith Parasite, emerged in England, affecting over 5,000 people with no apparent connection between them. The most common symptoms included fever and tiredness, but some infected individuals remained asymptomatic. The virus was associated with post-disease conditions such as loss of speech, confusion, chest pain, and shortness of breath. The transmission conditions and risk factors for the disease remained unknown, but some groups appeared more prone to infection than others.


# Objective


The goal of our project was to build a predictive model to answer the question, "Who are the people more likely to suffer from the Smith Parasite?". Our team had access to a small quantity of sociodemographic, health, and behavioral information from patients. As data scientists, we were tasked with analyzing and transforming the available data, and applying different models to accurately answer the defined question.


# Models applied: Hyper Parameters Table


0	Gradient Boosting	{'learning_rate': 0.5, 'loss': 'exponential', 'max_depth': 3, 'n_estimators': 200}


1	Ada Boosting	{'base_estimator': DecisionTreeClassifier(max_depth=2), 'learning_rate': 0.5, 'n_estimators': 300}


2	Random Forest	{'criterion': 'entropy', 'max_depth': None, 'max_features': 'sqrt', 'n_estimators': 100}


3	Logistic Regression	{'C': 1, 'penalty': 'l2'}


4	MLP	{'solver': 'sgd', 'max_iter': 500, 'learning_rate_init': 0.05, 'learning_rate': 'adaptive', 'hidden_layer_sizes': (50, 100, 50), 'alpha': 0.0001, 'activation': 'relu'}


5	Gaussian NB 	{'var_smoothing': 1.0}


6	LDA	{'solver': 'svd'}


7	KNN 	{'algorithm': 'ball_tree', 'n_neighbors': 1, 'weights': 'uniform'}


8	Randomized SVM	{'oob_score': True, 'n_estimators': 50, 'max_samples': 0.6, 'max_features': 0.8, 'bootstrap_features': False, 'bootstrap': True, 'base_estimator__kernel': 'rbf', 'base_estimator__C': 1}


9	Randomized LDA	{'oob_score': True, 'n_estimators': 80, 'max_samples': 0.7, 'max_features': 0.4, 'bootstrap_features': False, 'bootstrap': True, 'base_estimator__solver': 'svd'}


10	Randomized KNN	{'oob_score': False, 'n_estimators': 150, 'max_samples': 0.9, 'max_features': 0.3, 'bootstrap_features': False, 'bootstrap': True, 'base_estimator__weights': 'distance', 'base_estimator__n_neighbors': 4, 'base_estimator__algorithm': 'kd_tree'}


11	Randomized MLP	{'oob_score': True, 'n_estimators': 120, 'max_samples': 0.1, 'max_features': 0.7, 'bootstrap_features': False, 'bootstrap': True, 'base_estimator__solver': 'adam', 'base_estimator__max_iter': 400, 'base_estimator__learning_rate_init': 0.01, 'base_estimator__learning_rate': 'constant', 'base_estimator__hidden_layer_sizes': (50, 50, 50), 'base_estimator__alpha': 0.0001, 'base_estimator__activation': 'relu'}


12	Randomized Tree	{'oob_score': False, 'n_estimators': 80, 'max_samples': 0.3, 'max_features': 0.7, 'bootstrap_features': False, 'bootstrap': True, 'base_estimator__max_depth': 10, 'base_estimator__criterion': 'gini'}


13	Randomized Logit 	{'oob_score': False, 'n_estimators': 100, 'max_samples': 1.0, 'max_features': 0.6, 'bootstrap_features': False, 'bootstrap': True, 'base_estimator__penalty': 'l2', 'base_estimator__C': 1}


14	Randomized Gaussian NB	{'oob_score': False, 'n_estimators': 80, 'max_samples': 0.8, 'max_features': 0.9, 'bootstrap_features': True, 'bootstrap': True, 'base_estimator__var_smoothing': 4.3287612810830526e-07}


# Datasets
We had access to two different datasets:


Training Set: This set was used to build our machine learning models. It included the ground truth for each patient, i.e., if the patient had the disease (Disease = 1) or not (Disease = 0). The training set was composed of:


train_demo.csv - the training set for demographic data and the target


train_health.csv - the training set for health-related data


train_habits.csv - the training set for habits-related data


Test Set: This set was used to evaluate how well our model performed on unseen data. We didn't have access to the ground truth for this set, and our goal was to predict the disease status (0 or 1) using the model we created with the training set. The test set was composed of:

test_demo.csv - the test set for demographic data


test_health.csv - the test set for health-related data


test_habits.csv - the test set for habits-related data


# Evaluation


Our team's predictions were scored based on the percentage of instances we correctly predicted, using the f1 score. Our aim was to create a model that performed well on the test set and provided valuable insights into the factors influencing the likelihood of suffering from the Smith Parasite.
