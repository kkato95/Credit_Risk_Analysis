# Credit_Risk_Analysis

### Overview of the Analysis
We used imbalanced-learn and scikit-learn libraries on a dataset of loans and to evaluate models using resampling. We used RandomOverSampler and SMOTE algorithms and used ClusterCentroids to undersample the data. Then we used the combinatorial approach of over- and undersampling with SMOTEEN.
We then compared the new machinge learning models to reduce bias with BalancedRandomForestClassifier and EasyEnsembleClassifier.

#### We begin by:

Create Features and Target - Converted the string values to numerical using get_dummies().

![features_target](https://user-images.githubusercontent.com/99375741/176074225-22ccb317-d47a-4444-bf75-a0d1ca4c6482.png)


![train_data](https://user-images.githubusercontent.com/99375741/176075568-9536ba3e-ff6e-479b-9a2a-235808cafbf8.png)



### Results

1. Native Random Oversampling - 

The accuracy score is 0.657, which is a fair accuracy score. The model predicted true 65.7% of the time.
In the classfication report, this model shows a high-risk prediction score of 0.01, meaning if the model identified a loan was high-risk, it was actually high risk 1% of the time. The recall value is 0.71, indicating if the loan was high risk, it was identified 71% of the time. 

Accuracy Score:

![1_RandomOversampling_accuracy_score](https://user-images.githubusercontent.com/99375741/176062012-2f9a1b2e-3aa3-4c6c-ab92-04d991e148ea.png)


Classification Report:

![1_RandomOversampling_classification](https://user-images.githubusercontent.com/99375741/176062021-fc02c058-6402-48d3-adf5-da243eba742d.png)





2. SMOTE Oversampling - 

The accuarcy score is 0.653, which is a little less accurate than our RandomOverSampling model.
The precision is identical to the RandomOverSampling model. The recall value is .61, indicating SMOTE marked high risk correctly 61% of the time.

Accuracy Score:

![2_SMOTE_OverSampling_accuracy_score](https://user-images.githubusercontent.com/99375741/176062120-9feceaad-dc3e-477d-9114-634ee2138a85.png)


Classification Report:

![2_SMOTE_OverSampling_classification](https://user-images.githubusercontent.com/99375741/176062132-435769ab-6c81-4d45-ab5f-68f12e6c9dbf.png)





3. Undersampling - 

The Undersampling model shows an accuracy score of 0.653, very similar to the SMOTE model.
The precision is the same as the last two models with high-risk loans with a 0.01 precision for high-risk loans. The recall is .69 for high-risk loan.

Accuracy Score:

![3_Undersampling_accuracy_score](https://user-images.githubusercontent.com/99375741/176062225-239d8e61-fb94-4a4d-9a48-acce48d77a7f.png)


Classification Report:

![3_Undersampling_classification](https://user-images.githubusercontent.com/99375741/176062234-d144dc92-db15-40e9-848f-f739376bdba8.png)






4. Combination (Over and Under) Sampling

The accuracy score is fairly low at 0.544.
The precision is identical to all previous models. The recall for high-risk is fairly high at .72.

Accuracy Score:

![4_Combination_accuracy_score](https://user-images.githubusercontent.com/99375741/176062251-2fd5aa52-42c2-4da0-a74c-dcefcd11a139.png)


Classification Report:

![4_Combination_classification](https://user-images.githubusercontent.com/99375741/176062258-cde4cffb-a1a8-4f12-9771-9617954db7ab.png)






5. Balanced Random Forest Classifier -

The accuracy for the Random Forest Classifier high with a value of .789, indicating the model predicts correctly almost 70% of the time.
The precision is higher than the previous 4 models, with a precision of .03 for the high risk loans. The recall is high for both the high-risk and low-risk loans. The Balanced Random Forest Classifier is the best model yet.

Accuracy Score:

![5_BalancedRandomForest_accuracy_score](https://user-images.githubusercontent.com/99375741/176062285-090de4fa-5f2b-4abe-8841-b00deeea3b83.png)


Classification Report:

![5_BalancedRandomForest_classification](https://user-images.githubusercontent.com/99375741/176062293-fb6749d1-ec5b-4d67-a2be-ce22b1d3cf3d.png)






6. Easy Ensemble AdaBoost Classifier

The accuracy score is .931; Model is extremly accurate.
The precision score is 0.09 for the high-risk loans, meaning the score is 9x more precise the resampling models above.
Th recall is .92 for high_risk and .94 for low_risk.
The AdaBooth Classifier model is by far the best model for most all metrics we have analyzed.

Accuracy Score:

![6_AdaBoost_accuracy_score](https://user-images.githubusercontent.com/99375741/176062311-ac309494-e5c2-4c25-8337-6a4fe0868aad.png)


Classification Report:

![6_AdaBoost_classification](https://user-images.githubusercontent.com/99375741/176062349-fbf3756b-59b6-4632-b079-65db454b6b14.png)





#### Summary

In total, after running all 6 maching learning models, the ensemble models responded much more favorably than did the oversampling models. All the oversampling models had low accuracy scores, low precision scores and low recall scores. The AdaBoost Ensemble model far outpreformed every other model, with the highest accuracy, precision, and recall scores. The recommended model to use would be AdaBoost model. Althouhgh AdaBoost preformed the best, this model still had a 989 false positives out of 17k loans in the test data.
