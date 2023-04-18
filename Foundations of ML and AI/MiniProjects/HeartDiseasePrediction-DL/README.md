# Structured Data Classification

## Problem Statement
To predict whether a patient has a heart disease.

## Learning Objectives
At the end of the experiment, we will be able to:
- Understand the Cleveland Clinic Foundation for Heart Disease dataset.
- Pre-process this dataset using Keras layers: IntegerLookup, StringLookup & Normalization
- Understand and use Keras concatenate layer
- Build a neural network model and architecture using Keras functional api.
- Predict an unseen data.

## Introduction
This example demonstrates how to do structured data classification, starting from a raw CSV file. Our data includes both numerical and categorical features. We will use Keras preprocessing layers to normalize the numerical features and vectorize the categorical ones.
Note that this example should be run with TensorFlow 2.5 or higher.

## Dataset
Our dataset is provided by the Cleveland Clinic Foundation for Heart Disease. It's a CSV file with 303 rows. Each row contains information about a patient (a sample), and each column describes an attribute of the patient (a feature). We use the features to predict whether a patient has a heart disease (binary classification).
Here's the description of each feature:

- Age	Age in years	Numerical
- Sex	(1 = male; 0 = female)	Categorical
- CP	Chest pain type (0, 1, 2, 3, 4)	Categorical
- Trestbpd	Resting blood pressure (in mm Hg on admission)	Numerical
- Chol	Serum cholesterol in mg/dl	Numerical
- FBS	fasting blood sugar in 120 mg/dl (1 = true; 0 = false)	Categorical
- RestECG	Resting electrocardiogram results (0, 1, 2)	Categorical
- Thalach	Maximum heart rate achieved	Numerical
- Exang	Exercise induced angina (1 = yes; 0 = no)	Categorical
- Oldpeak	ST depression induced by exercise relative to rest	Numerical
- Slope	Slope of the peak exercise ST segment	Numerical
- CA	Number of major vessels (0-3) colored by fluoroscopy	Both numerical & categorical
- Thal	3 = normal; 6 = fixed defect; 7 = reversible defect	Categorical
- Target	Diagnosis of heart disease (1 = true; 0 = false)	Target
