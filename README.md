# Supervised Machine Learning 

## Challenge 
### Background 
Credit risk is an inherently unbalanced classification problem, as the number of good loans easily outnumber the number of risky loans. Therefore, we’ll need to employ different techniques to train and evaluate models with unbalanced classes. Our client asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Our final task is to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

### Objective
- Implement machine learning models.
- Use resampling to attempt to address class imbalance.
- Evaluate the performance of machine learning models.

### Summary of Analysis 
| Model | precision | recall | Accuracy score |
| :------  | :--: | :--: | :--: |
| Naive Random Oversampling | high-risk : 0.01 <br\> low-risk : 0.99 | high-risk : 0.67 <br\> low-risk : 0.63 | 0.648 | 
| SMOTE Oversampling | high-risk : 0.01 <br\> low-risk : 1.0 | high-risk : 0.62 <br\> low-risk : 0.68 | 0.649 | 
| ClusterCentroids Undersampling | high-risk : 0.01 <br\> low-risk : 1.0 | high-risk : 0.63 <br\> low-risk : 0.42 | 0.523 |
| SMOTEENN algorithm | high-risk : 0.01 <br\> low-risk : 1.0 | high-risk : 0.72 <br\> low-risk : 0.59 | 0.658 | 
| Balanced Random Forest Classifier | high-risk : 0.03 <br\> low-risk : 1.0 | high-risk : 0.61 <br\> low-risk : 0.88 | 0.745 | 
| Easy Ensemble AdaBoost Classifier | high-risk : 0.04 <br\> low-risk : 1.0 | high-risk : 0.88 <br\> low-risk : 0.88 | 0.881 |

- According to precision and recall scores, the Easy Ensemble AdaBoost Classifier performed better compare to 5 models we used to predict credit risk. However recall score of high-risk loan is 0.04, to predict high-risk loans we might need to research for a better prediction algorithm.  
