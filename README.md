# The Smith Parasite: Machine Learning Course Project - MDSAA-DS - Fall 2022


#Introduction


A newly discovered disease, identified as the Smith Parasite, emerged in England, affecting over 5,000 people with no apparent connection between them. The most common symptoms included fever and tiredness, but some infected individuals remained asymptomatic. The virus was associated with post-disease conditions such as loss of speech, confusion, chest pain, and shortness of breath. The transmission conditions and risk factors for the disease remained unknown, but some groups appeared more prone to infection than others.


# Objective


The goal of our project was to build a predictive model to answer the question, "Who are the people more likely to suffer from the Smith Parasite?". Our team had access to a small quantity of sociodemographic, health, and behavioral information from patients. As data scientists, we were tasked with analyzing and transforming the available data, and applying different models to accurately answer the defined question.


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


Evaluation


Our team's predictions were scored based on the percentage of instances we correctly predicted, using the f1 score. Our aim was to create a model that performed well on the test set and provided valuable insights into the factors influencing the likelihood of suffering from the Smith Parasite.
