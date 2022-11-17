# Credit_Risk_Analysis

## Overview of the analysis: 

This analysis attempts to predict the status of a loan based on a number of other factors. The analysis was performed by training several different supervised machine learning models and allowing these models to make predictions about loan status according to training experience. 

## Results: 

**Naive Random Oversampling**


![Screen Shot 2022-11-16 at 7 22 02 PM](https://user-images.githubusercontent.com/108832056/202323626-7673519a-78b3-4584-beff-e2ef1bbd15d2.png)

**SMOTE Oversampling**


![Screen Shot 2022-11-16 at 7 22 23 PM](https://user-images.githubusercontent.com/108832056/202323663-f65e8c5e-a025-424f-87d5-658e82de2e75.png)

**Undersampling**


![Screen Shot 2022-11-16 at 7 22 44 PM](https://user-images.githubusercontent.com/108832056/202323700-30b80e58-6ecf-4892-bd5c-245c1a309145.png)

**Combination (Over and Under) Sampling**


![Screen Shot 2022-11-16 at 7 23 07 PM](https://user-images.githubusercontent.com/108832056/202323733-89b05429-2d42-4280-93a1-b21766148479.png)

**Balanced Random Forest Classifier**


![Screen Shot 2022-11-16 at 7 23 41 PM](https://user-images.githubusercontent.com/108832056/202323795-b31bc571-c53f-47c3-a605-7fe3fd30c883.png)

**Easy Ensemble AdaBoost Classifier**


![Screen Shot 2022-11-16 at 7 24 03 PM](https://user-images.githubusercontent.com/108832056/202323835-8e270ae9-2fc7-491a-a8eb-998f160b1dc9.png)

Evidently, all models that were created had very high precision when it came to predicting low-risk loan status and low precision when it came to predicting high-risk loan status. Also, all models generally had much superior recall in predicting low-risk loan status compared to predicting high-risk loan status. All confusion matrices shown consist primarily of True Negatives (bottom right) that indicate low-risk loan status. Both of these make some sense because there was an extreme imbalance in the number of low-risk and high-risk loans in the data that was used. Despite attempts to curb this imbalance, such as over, under, or combined sampling, this imbalance can still sometimes come through. 

As the different models were being created, however, additional accuracy was gained. All oversampling, undersampling, and combined sampling models posted low accuracy scores ranging from 0.59 - 0.65. This suggested that these models were all relatively weak learners. Compared to these four models, the two ensemble classifiers, the random forest (0.79) and easy ensemble classifier (0.93), were much more accurate. Additionally, the recall for predicting high-risk loan status was much higher for the ensemble learners, with the easy ensemble classifier even having a 0.91 recall for high-risk loans and a 0.94 for low-risk loans. Clearly, the ensemble learners were far superior in their prediction.

## Summary: 

Overall, this analysis demonstrated how important it can sometimes be to combine many weak learners in order to create a stronger and more comprehensive predictive model. By far and away, the easy ensemble classifier was the most accurate supervised machine learning model that was created, and it predicted the status of loans in the dataset with considerable accuracy. 
