# Credit_Risk_Analysis

### Overview of the Analysis
We used imbalanced-learn and scikit-learn libraries on a dataset of loans and to evaluate models using resampling. We used RandomOverSampler and SMOTE algorithms and used ClusterCentroids to undersample the data. Then we used the combinatorial approach of over- and undersampling with SMOTEEN.
We then compared the new machinge learning models to reduce bias with BalancedRandomForestClassifier and EasyEnsembleClassifier.


### Results

1. Native Random Oversampling

Accuracy Score:

![1_RandomOversampling_accuracy_score](https://user-images.githubusercontent.com/99375741/176062012-2f9a1b2e-3aa3-4c6c-ab92-04d991e148ea.png)


Classification Report:

![1_RandomOversampling_classification](https://user-images.githubusercontent.com/99375741/176062021-fc02c058-6402-48d3-adf5-da243eba742d.png)



2. SMOTE Oversampling

Accuracy Score:

![2_SMOTE_OverSampling_accuracy_score](https://user-images.githubusercontent.com/99375741/176062120-9feceaad-dc3e-477d-9114-634ee2138a85.png)


Classification Report:

![2_SMOTE_OverSampling_classification](https://user-images.githubusercontent.com/99375741/176062132-435769ab-6c81-4d45-ab5f-68f12e6c9dbf.png)



3. Undersampling

Accuracy Score:
![3_Undersampling_accuracy_score](https://user-images.githubusercontent.com/99375741/176062225-239d8e61-fb94-4a4d-9a48-acce48d77a7f.png)


Classification Report:

![3_Undersampling_classification](https://user-images.githubusercontent.com/99375741/176062234-d144dc92-db15-40e9-848f-f739376bdba8.png)



4. Combination (Over and Under) Sampling

Accuracy Score:

![4_Combination_accuracy_score](https://user-images.githubusercontent.com/99375741/176062251-2fd5aa52-42c2-4da0-a74c-dcefcd11a139.png)


Classification Report:

![4_Combination_classification](https://user-images.githubusercontent.com/99375741/176062258-cde4cffb-a1a8-4f12-9771-9617954db7ab.png)



5. Balanced Random Forest Classifier

Accuracy Score:

![5_BalancedRandomForest_accuracy_score](https://user-images.githubusercontent.com/99375741/176062285-090de4fa-5f2b-4abe-8841-b00deeea3b83.png)


Classification Report:

![5_BalancedRandomForest_classification](https://user-images.githubusercontent.com/99375741/176062293-fb6749d1-ec5b-4d67-a2be-ce22b1d3cf3d.png)



6. Easy Ensemble AdaBoost Classifier

Accuracy Score:

![6_AdaBoost_accuracy_score](https://user-images.githubusercontent.com/99375741/176062311-ac309494-e5c2-4c25-8337-6a4fe0868aad.png)


Classification Report:

![6_AdaBoost_classification](https://user-images.githubusercontent.com/99375741/176062349-fbf3756b-59b6-4632-b079-65db454b6b14.png)



#### Summary

