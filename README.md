- ## Introduction

Goal is to compare the performance of the classifiers we encountered in this section, namely K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. We will utilize a dataset related to marketing bank products over the telephone.

Our dataset comes from the UCI Machine Learning repository link. The data is from a Portugese banking institution and is a collection of the results of multiple - marketing campaigns. We will make use of the article accompanying the dataset here for more information on the data and features.
 
## Objective
Our dataset comes from the UCI Machine Learning repository link. The data is from a Portugese banking institution and is a collection of the results of multiple -marketing campaigns. We will make use of the article accompanying the dataset here for more information on the data and features.
 
## Evaluated Models
Trained and tuned the following models:
 
- Logistic Regression
- KNNeighbors (KNN) 
- Decision Tree
- Support Vector Machine (SVM)
- XGBoost
- GradientBoosting
 
## Performance
 
| Model                        | Train Accuracy | Test Accuracy | CV Score            | 
|------------------------------|----------------|---------------|---------------------|
| Logistic Regression          | 91.0           | 90.0          | 0.9078907435508347  |
| KNNeighbors                  | 93.0           | 89.0          | 0.9018209408194233  |
| Decision Tree                | 100.0          | 88.0          | 0.8851896813353566  |
| Support Vector Machine       | 90.0           | 90.0          | 0.897481031866464   |
| XGBoost                      | 95.0           | 91.0          | 0.9111987860394537  |
| GradientBoosting             | 92.0           | 91.0          | 0.9154779969650987  |

## Highligts of Confusion Matrix

- False Positive, means the client do NOT SUBSCRIBED to term deposit, but the model thinks he did.
- False Negative, means the client SUBSCRIBED to term deposit, but the model said he dont.
- The first one its most harmful, because we think that we already have that client but we dont and maybe we lost him in other future campaings
- The second its not good but its ok, we have that client and in the future we'll identify that in truth he's already our client

## Recommendations
- SMOTE to be applied to solve Class imbalance
- After the analysis we see that our interest is over decreasing the False Negative means the client SUBSCRIBED to term deposit, but the model said he dont which indicates RECALL. So, we conclude that the model with high RECALL would be best suited for the problem statement

