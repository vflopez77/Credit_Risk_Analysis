# Credit Risk Analysis

## Overview
This analysis uses Machine Learning to classify risky loans by processing loan data.  If this can be achieved with accuracy, it would provide a more efficient way to approve or deny loans, and reduce the risk for the lending institution.  
A number of Machine Mearning models are tested to see which ones produced the best results.

## Results
The results and observations for the various models are outlined below.  Because the data set set is unbalanced i.e. there are far more low-risk records than high-risk ones, we will use oversampling and undersampling methods to find the best fit.

### Oversampling

#### Naive Random Oversampling
Balance Accuracy Score: 0.61439<br>
Confusion Matrix:<br>
<img src=Resources\NaiveRandomOversamplingCM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\NaiveRandomOversamplingICR.png></img><br>

#### SMOTE (Synthetic Minority Oversampling Technique) Oversampling
Balance Accuracy Score: 0.64573<br>
Confusion Matrix:<br>
<img src=Resources\SMOTE_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\SMOTE_ICR.png></img><br>

### Undersampling

#### ClusterCentroids
Balance Accuracy Score: 0.583145<br>
Confusion Matrix:<br>
<img src=Resources\CC_CM.png></img><br>
Imbalanced Classification Report:<br>
<img src=Resources\CC_ICR.png></img><br>
