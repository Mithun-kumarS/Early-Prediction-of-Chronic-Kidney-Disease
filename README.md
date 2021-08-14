# Early-Prediction-of-Chronic-Kidney-Disease

 Chronic Kidney disease (CKD) is the longstanding disease of the kidneys leading to renal failure. The model forecast whether the patient has invisible CKD or not, based on the medical test parameters - WBC Count, RBC Count, Urea level, blood glucose, &amp; other 22 variables. 
 
 The kidneys filter waste and excess fluid from the blood. As kidneys fail, waste builds up. Symptoms develop slowly and aren't specific to the disease. Some people have no symptoms at all and are diagnosed by a lab test. Medication helps manage symptoms. In later stages, filtering the blood with a machine (dialysis) or a transplant may be required
 
## About DataSet

Source : https://www.kaggle.com/mansoordaku/ckdisease

DataSet has 24 medical features + 1 class = 25 ( 11 numeric ,14 nominal)

## Data Cleaning

Below are the solved Challenges

Saved the dataType of { 'red blood cell count','packed cell volume','white blood cell count' } columns as numeric dataType.

Dropped the ID Column as it has no importance.

Corrected the misspelled data in categorical columns using replace() method 

Null_values in Numerical columns are filled using Random value Imputation method

Null_values in Categorical columns are filled using Random value Imputation & Mode imputation method


## Feature Selection
##### the top 10 important features are selected using information gain as per the below technique.

SelectKBest(score_func=chi2)

chi2 - Internally this class is going to check that whether p-value is less than 0.05 or not based on that,it will order all the features

## ML Models Used

CatBoostClassifier,
Logistic Regression,
Support Vector Machine,
Decision Tree,
Neural Network,
Random Forest,
XGBoost,
LGBMClassifier,
XGBRFClassifier,
GradientBoosting,
GaussianNB,
KNeighborsClassifier.

# Results-
![Untitled](https://user-images.githubusercontent.com/85584749/129441219-d86662ae-9a35-4e19-8275-481f6a467fbf.png)

## Sorted BarPlot of Accuracy

![Untitled](https://user-images.githubusercontent.com/85584749/129441394-5dc475c3-811a-427f-a236-850b7dbb9a75.png)

