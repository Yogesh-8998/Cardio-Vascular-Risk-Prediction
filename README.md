Cardiovascular Risk Prediction

The aim of this project is to predict heart disease using data mining techniques and machine learning algorithms. This project implements 3 classification models using scikit-learn: Logistic Regression, Support Vector Classifier, and boost Model to investigate their performance on heart disease dataset.

Data Discription

The data set is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes periods. The energy data was logged every 10 minutes with m-bus energy meters. Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes (parameters). factors.

Problem Statement

We have been given the cardiovascular data of nearly 3,300 people, where we have health characteristics. we want to make a machine learning model, which can learn from the pattern of these data and can predict if a person is going to have a cardiovascular risk in the next 10 years.

Data Summary

The dataset is publically available on the Kaggle website, and it is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes. Variables Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.

Demographic

Sex: male or female(Nominal)

Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)

Education: categorial feature (from 1 to 4)

Behavioral:

Current Smoker: whether or not the patient is a current smoker (Nominal)

Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.)

Information on medical history:

BP Meds: whether or not the patient was on blood pressure medication (Nominal)

Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)

Prevalent Hyp: whether or not the patient was hypertensive (Nominal)

Diabetes: whether or not the patient had diabetes (Nominal)

Information on current medical condition:

Tot Chol: total cholesterol level (Continuous)

Sys BP: systolic blood pressure (Continuous)

Dia BP: diastolic blood pressure (Continuous) *BMI: Body Mass Index (Continuous)

Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.)

Glucose: glucose level (Continuous)

Target variable to predict:

10-year risk of coronary heart disease (CHD) - (binary: “1”, means “Yes”, “0” means “No”)

Summary

As the first step, we understand the data & perform some cleaning on the null values, and checking the data types and EDA on data.

After EDA We divided our project into different model building and preprocessing before model.

As so we have a high imbalance data set, we used different techniques to balance the data like SMOTE and assign class weights.

We tried different models and evaluated their performance scores. Models Built: Logistic Regression, SVM, XGBoost

Based on our targeted evaluation metric - recall, we chose SVM as the suggested model
