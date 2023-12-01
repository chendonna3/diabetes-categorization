# Diabetes Prediction Using CDC Survey
Classifying diabetes project

### [Erdos Institute](https://www.erdosinstitute.org/) Data Science Boot Camp - Fall 2023

#### Team Members
- Donna Chen
- Gary Hu
- Michelle Lobb
- [Shayne Plourde](https://www.linkedin.com/in/shayne-plourde/)

## Project Overview
Diabetes is a major issue in the world, impacting 8.5% of adults and killing 1.5 million people in 2019 according to the World Health Organization. Diabetes is a chronic disease that affects how the body regulates blood glucose levels. Over time, having raised blood glucose levels may lead to serious damage to the nerves and blood vessels, leading to further complications. 

The goal of this project is to better understand the relationship between lifestyle factors and diabetes and subsequently predict whether an individual has diabetes or not, based on a survey questionnaire.



### Dataset used:
The Centers for Disease Control and Prevention annually collects a health-related telephone survey known as the Behavioral Risk Factor Surveillance System (BRFSS). This includes responses from over 400,000 Americans, containing healthcare statistics and lifestyle survey information, in addition to their diagnosis of diabetes. 

The Diabetes Health Indicators Dataset contains healthcare statistics and lifestyle survey information about people in general along with their diagnosis of diabetes. The 35 features consist of some demographics, lab test results, and answers to survey questions for each patient. The target variable for classification is whether a patient has diabetes, is pre-diabetic, or healthy.
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset/data



###  EDA results

The correlation between diabetes and the following characteristics was determined by a Spearman correlation >0.2:

 - HighBP
 - PhysHlth
 - DiffWalk
 - BMI
 - GenHlth
 - HighChol
 - HeartDiseaseorAttack
 - Age

There are 35346 diabetes, 4631 pre-diabetes patients, and 213703 patients without diabetes.
That's 13.93% diabetes and 1.83% pre-diabetes

## Results
The non-boosting methods for classification yielded accuracy scores capped at around 0.75, with the random forest model performing the best with 0.7562 accuracy, 0.7563 ROC AUC score, and 0.7961 recall on the balanced binary data set. The random forest model also provided relative importance scores for the features; the features with the highest importance scores were general health (0.2153), high blood pressure (0.2038), BMI (0.1279), age (0.1014), and high cholesterol (0.0937).
