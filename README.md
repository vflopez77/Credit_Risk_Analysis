# Credit Risk Analysis

## Overview
This analysis uses Machine Learning to classify risky loans by processing loan data.  If this can be achieved with accuracy, it would provide a more efficient way to approve or deny loans, and reduce the risk for the lending institution.  
A number of different Machine Mearning models were tested to see which ones produced the best outcome.

## Results
The results and observations for the various models are outlined below.  Because the data set set is unbalanced i.e. there are far more low-risk records than high-risk ones, we will use oversampling and undersampling methods to find the best fit.

### Oversampling

#### Naive Random Oversampling
- Balanced Accuracy Score: 0.61439<br>
- Confusion Matrix:<br>
<img src=Resources\NaiveRandomOversamplingCM.png></img><br>
- Imbalanced Classification Report:<br>
<img src=Resources\NaiveRandomOversamplingICR.png></img><br>

#### SMOTE (Synthetic Minority Oversampling Technique) Oversampling
- Balanced Accuracy Score: 0.64573<br>
- Confusion Matrix:<br>
<img src=Resources\SMOTE_CM.png></img><br>
- Imbalanced Classification Report:<br>
<img src=Resources\SMOTE_ICR.png></img><br>

### Undersampling

#### Cluster Centroids
- Balanced Accuracy Score: 0.583145<br>
- Confusion Matrix:<br>
<img src=Resources\CC_CM.png></img><br>
- Imbalanced Classification Report:<br>
<img src=Resources\CC_ICR.png></img><br>


### Combination Sampling

#### SMOTEENN (SMOTE with Edited Nearest Neighbor) Sampling
- Balanced Accuracy Score: 0.54044<br>
- Confusion Matrix:<br>
<img src=Resources\SMOTEENN_CM.png></img><br>
- Imbalanced Classification Report:<br>
<img src=Resources\SMOTEENN_ICR.png></img><br>

### Ensemble Learners

#### Random Forest Classifier
- Balanced Accuracy Score: 0.66632<br>
- Confusion Matrix:<br>
<img src=Resources\RF_CM.png></img><br>
- Imbalanced Classification Report:<br>
<img src=Resources\RF_ICR.png></img><br>

#### Easy Ensemble Adaptive Boost Classifier
- Balanced Accuracy Score: 0.68378<br>
- Confusion Matrix:<br>
<img src=Resources\EE_CM.png></img><br>
- Imbalanced Classification Report:<br>
<img src=Resources\EE_ICR.png></img><br>

## Summary
### Over- and Under-Sampling Models
- <b>SMOTE</b> did relatively well with a Balanced Accuracy of 0.65, Precision of 0.99, Recall of 0.68 and a Specificity (important for unbalanced data sets) of 0.61.
- <b>SMOTEENN</b> (SMOTE with Edited Nearest Neighbor) was the worst of the group with a Balanced Accuracy Score of 0.54, Precision of 0.99, Recall of 0.59, and Specificity of 0.49.
- <b>Naive Random Oversampling</b> was the second best in this group with a Balanced Accuracy Score of 0.62, Precision of 0.99, Recall of 0.67, and specificity of 0.56.
- <b>Cluster Centroids Undersampling</b> was the second worst in this group with Balanced Accuracy Score of 0.58, Precision of 0.99, recall of 0.39, and Specificity of 0.78.

### Ensemble Learners
- <b>Random Forest Classifier</b> did better than any of the Over- and Under-sampling models with a Balanced Accuracy Score: 0.67, Precision of 1.0, Recall of 1.0, and Specificity of 0.34.
- <b>Easy Ensemble Adaptive Boost Classifier</b> did better than any of the other models with a Balanced Accuracy of 0.68, Precision of 0.99, Recall of 0.73 and a Specificity of 0.63.

*(Note that Precision in such an unbalanced data set is not particularly significant).





