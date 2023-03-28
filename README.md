# TheSmithParasite

Machine Learning Project 2022-2023
The Smith Parasite

The goal is to build a predictive model that answers the question, “Who are the people more likely to suffer from the Smith Parasite?”.

With that goal, we were fiven access to a small quantity of sociodemographic, health, and behavioral information obtained from the patients. We had to analyze and transform the data available as needed and apply different models to answer the defined question in a more accurate way.

//The score of the predictions is the percentage of instances we correctly predict, using the f1 score.//

Data used 


train_demo.csv - the training set for demographic data and the target

train_health.csv - the training set for health related data

train_habits.csv - the training set for habits related data

test_demo.csv - the test set for demographic data

test_health.csv - the test set for health related data

test_habits.csv - the test set for habits related data

Submission
sampleSubmission.csv - a sample submission file in the correct format

Data fields
Sociodemographic Data
PatientID - The unique identifier of the patient

Birth_Year - Patient Year of Birth

Name - Name of the patient

Region - Patient Living Region

Education - Answer to the question: What is the highest grade or year of school you have?

Disease - The dependent variable. If the patient has the disease (Disease = 1) or not (Disease = 0)

Health Related Data
PatientID - The unique identifier of the patient

Height - Patient's height

Weight - Patient's weight

Checkup - Answer to the question: How long has it been since you last visited a doctor for a routine Checkup? [A routine Checkup is a general physical exam, not an exam for a specific injury, illness, or condition.]

Diabetes - Answer to the question: (Ever told) you or your direct relatives have diabetes?

High_Cholesterol - Cholesterol value

Blood_Pressure - Blood Pressure in rest value

Mental Health - Answer to the question: During the past 30 days, for about how many days did poor physical or mental health keep you from doing your usual activities, such as self-care, work, or recreation?

Physical Health - Answer to the question: Thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 days was your physical health not good to the point where it was difficult to walk?

Habits Related Data
PatientID - The unique identifier of the patient

Smoking_Habit - Answer to the question: Do you smoke more than 10 cigars daily?

Drinking_Habit - Answer to the question: What is your behavior concerning alcohol consumption?

Exercise - Answer to the question: Do you exercise (more than 30 minutes) 3 times per week or more?

Fruit_Habit - Answer to the question: How many portions of fruits do you consume per day?

Water_Habit - Answer to the question: How much water do you drink per day?
