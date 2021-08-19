# Credit_Risk_Analysis

## Overview of the Analysis: 

The purpose of this Loan Prediction Risk Analysis is to assess which of the six (6) supervised machine learning models performs better in predicting and classifying data to determine which customer loan applicants would be high or low risk investments.  

## Results: 

![image](https://user-images.githubusercontent.com/79073778/130117004-2511d7b5-9035-41bb-8029-5b463aa31f16.png)

*Note additional Classification Reports in Appendix below.	

__Balanced Accuracy Score (BAS)__
* Four models (Naive Random Oversampling, Smote Oversampling, Undersampling and SMOTEENN) had a **BAS** score range between 81% and 84% signaling these models were accurate and high performing. 
* Three out of 4 of those models had the exact same BAS score of 84%.  
* The models with the highest and lowest **BAS** score were Easy Ensemble Classifier (93%) and Random Forest Classifier (68%), respectively.  
* The low **BAS** score (68%) for the Random Forest Classifier suggests that the model did not perform well with classifying it's predictions. 

__Predictions (PRE)__
* Four out of 6 models (Naive Random Oversampling, Smote Oversampling, Undersampling, SMOTEENN) had a **PRE** score range between 0.02 and 0.03 signaling the low probability and reliability of positive classifications and indicative of a large number of false positives noted in their confusion matrices. 
* The Easy Ensemble Classifier posted a **PRE** score of .09 that is roughly inline with the aforementioned models. 
* The outlier was the Random Forest Classifier that produced a calculated **PRE** score of 0.88 that would suggest a large number of false positives. 
* When coupling the Random Forest's low **BAS** score and it's high **PRE** score, these measurements are incongruent with each other suggesting the **PRE** score may be a misleading measure.

__Recall (REC)__
* The **REC** measurement for all 6 models follow a similar trend as the **BAS** scores.
* Four models measure (high risk/low risk) inline with each other: Naive Random Oversampling (0.83/0.84), Smote Oversampling (0.81/0.87), Undersampling (0.86/0.76) and SMOTEENN (0.83/0.86). This high measurement scores for the binary prediction were likely correctly classified.
* The models with the highest and lowest **REC** score were Easy Ensemble Classifier (0.92/0.94) and Random Forest Classifier (0.37/1.00), respectively.
* The Random Forest Classifier's low **PRE** hi-risk score of 0.37 highlights the large number of false positives derived from model and its confusion matrix.   

## Summary: 

Five out of the 6 models proved worthy of using as a loan prediction analysis tool. The measurements of all 5 models with the exception of Random Forest, were all in line with each other.  That suggested to me a high probability that the models were analyzing the data similarly. The measurment scores for the Random Forest Classification model persisted in being opposite of all the other 5 models.  Perhaps this was an issue because of the small training and test samples of the data.  

However, I found that the **Easy Ensemble Classifier (EEC)** had the higher measurement scores among the five adequate models.  **EEC**'s classification of data was distributed among the True Positive and True Negative categories lending support to it's high **BAS** score. I recommend the Easy Ensemble Classifier as the model to use.


### Appendix of Classification Reports
*Naive Random Oversampling

![image](https://user-images.githubusercontent.com/79073778/129509988-a9642c43-169d-42d7-8663-5c8e2c544f2b.png)

*Smote Oversampling

![image](https://user-images.githubusercontent.com/79073778/129510116-63c1c210-2f0c-4773-a12b-e9cbb37a0c3c.png)

*Undersampling

![image](https://user-images.githubusercontent.com/79073778/129510201-7dc0d74b-712a-40bc-94fc-bf6566fe8ff2.png)

*Combination (Over & Under) Sampling/SMOTEENN

![image](https://user-images.githubusercontent.com/79073778/129510383-a6aaa341-b2a0-4da2-ab21-906bcc0dbafe.png)

*Random Forest Classifier

![image](https://user-images.githubusercontent.com/79073778/129510509-6025a601-0216-4fed-9b1e-d7ffc929ed0f.png)

*Easy Ensemble Classifier

![image](https://user-images.githubusercontent.com/79073778/129510735-d05161c7-0cf8-48e6-a681-cd5c3103a780.png)







