# Cardiovascular-Risk-prediction
# Problem statement
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham,Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes
over 4,000 records and 15 attributes.Variables

> Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk
factors.

# Data Description

> Demographic:

> • Sex: male or female("M" or "F")

> • Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)

>Behavioral

> • is_smoking: whether or not the patient is a current smoker ("YES" or "NO")

> • Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.)

> Medical( history)

> • BP Meds: whether or not the patient was on blood pressure medication (Nominal)


> • Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)

> • Prevalent Hyp: whether or not the patient was hypertensive (Nominal)

> • Diabetes: whether or not the patient had diabetes (Nominal)
Medical(current)

> • Tot Chol: total cholesterol level (Continuous)

> • Sys BP: systolic blood pressure (Continuous)

> • Dia BP: diastolic blood pressure (Continuous)

> • BMI: Body Mass Index (Continuous)

> • Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though infact discrete, yet are considered continuous because of large number of possible values.)

> • Glucose: glucose level (Continuous)

> Predict variable (desired target)

> • 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”) -
DV

# Project summary

* Currently cardiovascular diseases (CVDs) are the main cause of death worldwide. 
Disease risk estimates can be used as prognostic information and support for treating CVDs. 

* The commonly used Framingham risk score (FRS) for CVD prediction is outdated for the modern population, so FRS may not be accurate enough.

* In this project ,a  CVD prediction system based on machine learning is proposed.

* The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 3,000 records and 15 attributes.

* Each attribute is a potential risk factor. There are  demographic, behavioral, and medical risk factors.

* Various ML models were built to predict weather a person will have CVD in 10 years or not and the performance of the model was checked against various metrics. 
# Conclusions


Conclusions based on EDA-
 
1)Males are more prone to CHD  as compared to females.
 
2)Smokers are more prone to CHD as compared to non smokers though it makes only a little difference.
 
3)People on BP medications are more prone to CHD.
 
4)People who had any previous prevalent stroke are more prone to having CHD although people who had prevalent stroke are very less.
 
5)Those who have prev hyp are more prone to having CHD.
 
6)Those who have diabetes are also more prone to having CHD although the number of people who have diabetes are very less.
7)Median age of people who have CHD is higher as compared to people who don't have CHD.This implies that people having a higher age are more prone to having CHD.
 
8)People who had CHD smoke more cigarettes as compared to people who had no CHD.
 
9)people who have CHD have more tot chol,sysBP,diaBP,BMI.

Conclusions based on model performances-

1)Ensemble models are performing better as compared to other models with adaboost being the best performing model followed by stacking and bagging.

2)We can see from the evaluation metric table that the best performing model is adaboost classifier because it has the best accuracy and has the highest recall as well.

3)In this type of problem our priority should be to reduce the number of False Negatives or find maximum Recall score. If we misclassify someone as having no risk of heart disease, it can be highly detrimental, it can lead to loss of life. Adaboost gives us an excellent Recall and at the same time doesn't compromise on Precision. If we require a model with more strict Recall values we can opt for KNN.


