# Cardiovascular-Risk-Prediction

                                                     Cardiovascular Risk Prediction
                                                       Contributor: Vibha Kumari
                                                      
Introduction:
Predicting coronary heart disease in advance helps raise awareness for the disease. Preventive measurements like changing diet plans and exercise can slow down the progression of CHD. Early prediction can result in early diagnosis. So, we can treat the disease at an early stage and avoid more invasive treatment.
Problem Statement:
The goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD).
Data Description:
The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes. Variables Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors
Demographic:
• Sex: male or female ("M" or "F")
• Age: Age of the patient
Behavioral:
• is smoking: whether or not the patient is a current smoker ("YES" or "NO")
• Cigs Per Day: the number of cigarettes that the person smoked on average in one day
Medical (History):
• BP Meds: whether or not the patient was on blood pressure medication
• Prevalent Stroke: whether or not the patient had previously had a stroke
• Prevalent Hyp: whether or not the patient was hypertensive
• Diabetes: whether or not the patient had diabetes (Nominal) Medical(current)
• Tot Chol: total cholesterol level
• Sys BP: systolic blood pressure
• Día BP: diastolic blood pressure
• BMI: Body Mass Index
• Heart Rate: heart rate
• Glucose: glucose level
• CHD: 10-year risk of coronary heart disease CHD (binary: “1”, means “Yes”, “0” means “No”)


Approach:
-
•	Data preparation:
• Removed null values from the dataset
• Removed duplicate entries
• Used SMOTE and random under sampling to get a balanced dataset
Pulse Pressure = Systolic BP - Diastolic BP

Model Used:

•	  Logistic Regression   
•	  K Nearest Neighbours   
•	  Naive Bayes       
•	  Decision Tree      
•	Support Vector Machines

 Conclusions:
 
1 . I trained 5 Machine Learning models using the training dataset, and hyperparameter tuning was used in some models to improve the model performance.

2. To build the models, missing values were handled, feature engineering and feature selection was performed, and the training dataset was oversampled using SMOTE to reduce bias on one outcome.

3. Recall was chosen as the model evaluation metric because it was very important that we reduce the false negatives.

4. Initial set of predictions were obtained using the baseline model, i.e., logistic regression model, and other commonly used classification models were also built in search of better predictions.

5. Predicting the risk of coronary heart disease is critical for reducing fatalities caused by this illness. We can avert deaths by taking the required medications and precautions if we can foresee the danger of this sickness ahead of time.

6. It is critical that the model we develop has a high recall score. It is OK if the model incorrectly identifies a healthy patient as a high-risk patient because it will not result in death, but if a high-risk patient is incorrectly labelled as healthy, it may result in fatality.

7. We were able to create a model with a recall of just 0.77 because of limited data available and limited computational power available.

8. A recall score of 0.77 indicates that out of 100 individuals with the illness, our model will be able to classify only 77 as high-risk patients, while the remaining 33 will be misclassified.

9. Future developments must include a strategy to improve the model recall score, enabling us to save even more lives from this disease. This includes involving more people in the study, and include people with different medical history, etc. build an application with better recall score.

10. From our analysis, it is also found that the age of a person was the most important feature in determining the risk of a patient getting infected with CHD, followed by pulse pressure, prevalent hypertension and total cholesterol. Diabetes, prevalent stroke and BP medication were the least important features in determining the risk of CHD.
