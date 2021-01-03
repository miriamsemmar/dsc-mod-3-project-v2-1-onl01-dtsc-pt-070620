
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

- Then, we tested multiple algorithms and narrowed our focus to three. 
- We then used these three algorithms to perform GridSearchCV in order to improve the model performance.


# Final Model

The main goal of this project is to create a classification model. For this project you have the choice to either:

- choose a data set from a curated list
- choose your own data set _outside_ of the curated list. 

The data guidelines for either option are shown below

For this project, you're going to select a dataset of your choosing and create a classification model. You'll start by identifying a problem you can solve with classification, and then identify a dataset. You'll then use everything you've learned about Data Science and Machine Learning thus far to source a dataset, preprocess and explore it, and then build and interpret a classification model that answers your chosen question.

# Recommendations & Next Steps

You are allowed to select one of the four data sets described below. Each comes with its own advantages and disadvantages, and, of course, its own associated business problem and stakeholders. It may be desirable to flesh out your understanding of the audience or the business proposition a little more than sketched out here. If you select one of these four data sets, you **need no further approval from your instructor**.


1) [Chicago Car Crash Data](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if). Note this links also to [Vehicle Data](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Vehicles/68nd-jvt3) and to [Driver/Passenger Data](https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d).
