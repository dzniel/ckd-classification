# Chronic Kidney Disease Classification

This repository contains a simple machine learning project of mine that looks into classifying whether a given data about someone indicates that they might have chronic kidney disease or not by implementing _k-Nearest Neighbors_ from scratch.

## Context
Chronic Kidney Disease is a long-term condition where kidneys do not work as well as they should. This disease can only get worse over time and eventually fail the kidneys. However, it is possible to diagnose this disease through blood test and urine test.

Read more: https://en.wikipedia.org/wiki/Chronic_kidney_disease

## Data
The data used for training and testing the machine learning model is taken from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/chronic_kidney_disease) which comes with 400 entries and 25 attributes.

__Issues identified within the provided data__
1. Short column names that could be hard to interpret
2. Incorrect data type for some numerical attributes
3. Incorrect values for some categorical attributes
4. Categorical attribute incompatible for predictive modeling
5. Numerous missing values spread across the 

__Issues handling__
1. Rename every columns for much easier interpretation
2. Convert attributes to its suitable data type
3. Remove anomaly in categorical attribute values
4. Transform categorical attributes to numeric attributes
5. Scale and impute data with KNNImputer

With the given amount of data, it is more ideal to split the data into 60-20-20 split. Where 60% of the data will be for training, 20% of the data will be for validating, and 20% of the data left will be for testing. The main purpose is to ensure our model generalize as well as possible.

## Methodology
The methodology used to perform predictive modeling is the k-Nearest Neighbors. The model itself is very simple yet can also be very effective for classifying data based on distance. With this model, it is crucial to figure out the optimal number of neighbors so more accurate classification will be achieved.

## Conclusion
Although there are still a lot of improvements to be made for this experimentation, however the k-Nearest Neighbors still did a great job classifying the disease as shown through the [experimentation notebook](https://github.com/dzniel/ckd-classification/blob/main/ckd_classification.ipynb).
