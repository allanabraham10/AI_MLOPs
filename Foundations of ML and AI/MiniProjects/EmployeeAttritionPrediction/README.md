# Employee Attrition Prediction using Boosting Techniques

## Problem Statement
To predict employee attrition using CatBoost and XgBoost

## Learning Objectives
At the end of the experiment, we will be able to:
- explore the employee attrition dataset
- apply CatBoost and XgBoost on the dataset
- tune the model hyperparameters to improve accuracy
- evaluate the model using suitable metrics

## Introduction
Employee attrition is the gradual reduction in employee numbers. Employee attrition happens when the size of your workforce diminishes over time. This means that employees are leaving faster than they are hired. Employee attrition happens when employees retire, resign, or simply aren't replaced. Although employee attrition can be company-wide, it may also be confined to specific parts of a business.
Employee attrition can happen for several reasons. These include unhappiness about employee benefits or the pay structure, a lack of employee development opportunities, and even poor conditions in the workplace.

### Gradient Boosted Decision Trees

Gradient boosted decision trees (GBDTs) are one of the most important machine learning models.
GBDTs originate from AdaBoost, an algorithm that ensembles weak learners and uses the majority vote, weighted by their individual accuracy, to solve binary classification problems. The weak learners in this case are decision trees with a single split, called decision stumps.
Some of the widely used gradient boosted decision trees are XgBoost, CatBoost and LightGBM.

## Dataset
The dataset used for this mini-project is HR Employee Attrition dataset. This dataset is synthetically created by IBM data scientists. There are 35 features and 1470 records.

There are numerical features such as:
- Age
- DistanceFromHome
- EmployeeNumber
- PerformanceRating

There are several categorical features such as:
- JobRole
- EducationField
- Department
- BusinessTravel

Dependent or target feature is 'attrition' which has values as Yes/No.
