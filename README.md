
# Module 3 Final Project


## Introduction

T-Comm, a telecommunications business, contacted us to better understand why some of their customers churn (essentially, end their phone plans). For this analysis, we leveraged machine learning algorithms and the data provided. Example customer features include daily call minutes, whether or not a customer bought an international plan and the number of times customer service was contacted. Our primary KPI was recall because we are most concerned with correctly predicting the number of churned customers.

## The Data

For this project, we leveraged data from [Kaggle](https://www.kaggle.com/becksddf/churn-in-telecoms-dataset).

# Approach

- We started out by cleaning our data, scaling our data and handling class imbalance. 

<p align="center">
  <img src="https://github.com/miriamsemmar/dsc-mod-3-project-v2-1-onl01-dtsc-pt-070620/blob/master/Churn%20Proportion.png" />
</p>

- Then, we tested multiple algorithms and narrowed our focus to three algorithms. We moved forward with the three algorithms with the highest recall scores, ignoring Decision Trees because the precision score was very low.  

<p align="center">
  <img src="https://github.com/miriamsemmar/dsc-mod-3-project-v2-1-onl01-dtsc-pt-070620/blob/master/Baseline%20Models.png" />
</p>

- We then used these three algorithms to perform GridSearchCV in order to improve the model performance.


# Final Model

Our XGBoost model using GridSearch CV was our best resulting model. We were able to improve all 4 scoring metrics, settling on a final model with 78% recall and 94% accuracy.

<p align="center">
  <img src="https://github.com/miriamsemmar/dsc-mod-3-project-v2-1-onl01-dtsc-pt-070620/blob/master/Final%20Model%20Scores.png" />
</p>

Interpretation: our model is correctly predicted churn 78% of the time. The model correctly guessed customer behavior with 94% accuracy.

<p align="right">
  <img src="https://github.com/miriamsemmar/dsc-mod-3-project-v2-1-onl01-dtsc-pt-070620/blob/master/Final_Model.png" />
</p>
 
 
 ## Feature Importance
 
 We used SHAP to help detrmine feature importance. 
 
 <p align="right">
  <img src="https://github.com/miriamsemmar/dsc-mod-3-project-v2-1-onl01-dtsc-pt-070620/blob/master/SHAP_Feature_Importance.png" width="600" />
</p>
 
- Number of customer service calls
 - Customers with a high number of customer service calls are more likely to churn
- Number of daily call minutes and evening minutes
 - The higher the number of minutes, the more likely a customer is to churn
- Users without an international plan are less likely to churn
- Users without an voicemail plan are more likely to churn


# Recommendations & Next Steps

We’d recommend recreating the model with some our strongest features to try to improve our recall score. 

With the information we have, we recommend evaluating the current plan types offered. The high correlation between call time and churn may indicate that customers need more plan flexibility. Consider adding unlimited plans to the current lineup. We can also test including voicemail plans as a part of these plans. 

We also need to further investigate the effectiveness of our current customer service offerings. Moreover, we should be considering offering discounts or incentives to unhappy customers who contact us in order to help improve the relationship.
