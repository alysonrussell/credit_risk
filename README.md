# Credit Risk Analysis

This exercise explores several different options for predicting credit risk and will advise whether each should be used for this purpose.



#### Process

Data was manipulated using:

- Oversampling using RandomOverSampler
- Oversampling using SMOTE algorithm
- Undersampling using cluster centroids
- Combination over/under sampling using SMOTEENN



#### Outcome

|                     | Precison Score | Recall Score | Balanced Accuracy Score |
| ------------------- | :------------: | :----------: | :---------------------: |
| Random Oversampling |      0.99      |     0.71     |          0.72           |
| SMOTE Oversampling  |      0.99      |     0.70     |          0.70           |
| Undersampling       |      0.99      |     0.48     |          0.64           |
| SMOTEENN            |      0.99      |     0.68     |          0.70           |



#### Recommendation

Since the vast majority of credit applications are low-risk, we see that the Precision Score for all models is almost perfect.  We see the best Recall Score for the Oversampling models.  The overall best Balanced Accuracy Score is found with Random Oversampling, although SMOTE Oversampling and SMOTEENN are tied very close behind.  I would prefer a higher accuracy score for determining loan eligibility, especially on higher dollar amounts, but in the options provided here I would suggest going with the Random Oversampling option.