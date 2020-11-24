# Credit Risk Analysis

## Overview
This analysis uses Machine Learning to classify risky loans by processing loan data.  If this can be achieved with accuracy, it would provide a more efficient way to approve or deny loans, and reduce the risk for the lending institution.  
A number of Machine Mearning models are tested to see which ones produced the best results.

## Results
The results and observations for the various models are outlined below.  Because the data set set is unbalanced i.e. there are far more low-risk records than high-risk ones, we will use oversampling and undersampling methods to find the best fit.

### Oversampling

#### Naive Random Oversampling
Balanced Accuracy Score: 0.61439<br>
Confusion Matrix:<br>
<img src=Resources\NaiveRandomOversamplingCM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\NaiveRandomOversamplingICR.png></img><br>

#### SMOTE (Synthetic Minority Oversampling Technique) Oversampling
Balanced Accuracy Score: 0.64573<br>
Confusion Matrix:<br>
<img src=Resources\SMOTE_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\SMOTE_ICR.png></img><br>

### Undersampling

#### ClusterCentroids
Balanced Accuracy Score: 0.583145<br>
Confusion Matrix:<br>
<img src=Resources\CC_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\CC_ICR.png></img><br>


### Combination Sampling

#### SMOTEENN (SMOTE with Edited Nearest Neighbor) Sampling
Balanced Accuracy Score: 0.54044<br>
Confusion Matrix:<br>
<img src=Resources\SMOTEENN_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\SMOTEENN_ICR.png></img><br>

### Ensemble Learners

#### Random Forest Classifier
Balanced Accuracy Score: 0.66632<br>
Confusion Matrix:<br>
<img src=Resources\RF_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\RF_ICR.png></img><br>

#### Easy Ensemble Adaptive Boost Classifier
Balanced Accuracy Score: 0.68378<br>
Confusion Matrix:<br>
<img src=Resources\EE_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\EE_ICR.png></img><br>

## Summary
There are some clear lessons to be drawn from this analysis.  Of the over- and under-sampling models, <b>SMOTE</b> did relatively well with a Balanced Accuracy of 0.65 and a Combined Specificity (imortant for unbalanced data sets) of 0.61.
The real standout, however, was the <b>Easy Ensemble Adaptive Boost Classifier</b> with a Balanced Accuracy of 0.68 and a Combined Specificity of 0.63.



