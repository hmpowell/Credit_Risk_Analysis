# Credit_Risk_Analysis

## Overview of the analysis

The purpose of this analysis was to use several techniques to train and evaluate models with unbalanced classes because we are evaluating credit risk for loan disbursement. We utilized oversampling, undersampling, combination sampling, and two machine learning models that reduce bias.

## Results

#### Naive Random Oversampling
- Balanced Accuracy: 0.65

![This is a photo of the code and results of the balanced accuracy score for the Naive Random Oversampling model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling_balanced_accuracy.png)

- Precision:
    - High risk - 0.01 (Poor)
    - Low risk - 1.00
- Recall: 
    - High risk - 0.72
    - Low risk - 0.59 (Poor)

![This is a photo of the code and results of the classification report for the naive random oversampling model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling_classification.png)

#### SMOTE Oversampling
- Balanced Accuracy: 0.66

![This is a photo of the code and results of the balanced accuracy score for the SMOTE Oversampling model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling_balanced_accuracy.png)

- Precision:
    - High risk - 0.01 (Poor)
    - Low risk - 1.00 (Excellent)
- Recall: 
    - High risk - 0.63 (Poor)
    - Low risk - 0.69 (Satisfactory)

![This is a photo of the code and results of the classification report for the SMOTE Oversampling model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling_classification.png)

#### Undersampling
- Balanced Accuracy: 0.58

![This is a photo of the code and results of the balanced accuracy score for the Undersampling model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Undersampling_balanced_accuracy.png)

- Precision:
    - High risk - 0.01 (Poor)
    - Low risk - 1.00 (Excellent)
- Recall: 
    - High risk - 0.61 (Poor)
    - Low risk - 0.55 (Poor)
    
![This is a photo of the code and results of the classification report for the Undersampling model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Undersampling_classification.png)

#### SMOTEENN
- Balanced Accuracy: 0.65

![This is a photo of the code and results of the balanced accuracy score for the SMOTEENN model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_balanced_accuracy.png)

- Precision:
    - High risk - 0.01 (Poor)
    - Low risk - 1.00 (Excellent)
- Recall: 
    - High risk - 0.72 (Satisfactory)
    - Low risk - 0.57 (Poor)
    
![This is a photo of the code and results of the classification report for the SMOTEENN model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_classification.png)

#### Balanced Random Forest Classifier
- Balanced Accuracy: 0.79

![This is a photo of the code and results of the balanced accuracy score for the Balanced Random Forest Classifier model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest_balanced_accuracy.png)

- Precision:
    - High risk - 0.03 (Poor)
    - Low risk - 1.00 (Excellent)
- Recall: 
    - High risk - 0.70 (Satisfactory)
    - Low risk - 0.87 (Great)
    
![This is a photo of the code and results of the classification report for the Balanced Random Forest Classifier model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest_classification.png)

#### Easy Ensemble AdaBoost Classifier
- Balanced Accuracy: 0.93

![This is a photo of the code and results of the balanced accuracy score for the Easy Ensemble AdaBoost Classifier model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost_balanced_accuracy.png)

- Precision:
    - High risk - 0.09 (Poor)
    - Low risk - 1.00 (Excellent)
- Recall: 
    - High risk - 0.92 (Excellent)
    - Low risk - 0.94 (Excellent)
    
![This is a photo of the code and results of the classification report for the Easy Ensemble AdaBoost Classifier model.](https://github.com/hmpowell/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost_classification.png)

## Summary

In the above models, we were able to calculate how well the models accurately predicted whether or not someone was a high risk loan applicant or a low risk loan applicant. The highest balanced accuracy came from the Easy Ensemble AdaBoost Classifier. If I was forced to choose a model, it would be that one; however, it has a very low precision level when it comes to predicting high risk loan applicants. With that low precision, we can determine that those we deem high risk are, in fact, high risk; however, there may be many more high risk applicants who are falsely determined to be low risk. Every one of these models had a low precision score for high risk, which leads me to not recommend any of these models for use in this case. 