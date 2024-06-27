# Insurance Claims Prediction

This project demonstrates how to handle imbalanced data and perform classification on an insurance claims dataset using Python. The goal is to predict whether an insurance claim will be made (1) or not (0).

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Handling Class Imbalance](#handling-class-imbalance)
- [Feature Selection](#feature-selection)
- [Model Training](#model-training)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

This project addresses the challenge of class imbalance in insurance claims data by using oversampling techniques and building a Random Forest classifier to predict the claim status.

## Dataset

The dataset contains 58,592 entries and 41 columns, including the target variable `claim_status`.

- **policy_id:** Unique identifier for the insurance policy
- **subscription_length, vehicle_age, customer_age:** Numeric attributes related to the policy, vehicle, and customer
- **region_code, segment, model, fuel_type:** Categorical attributes representing the region, vehicle segment, model, and fuel type
- **max_torque, max_power, engine_type:** Specifications of the vehicle’s engine
- **airbags, is_esc, is_adjustable_steering:** Features related to the vehicle’s safety and convenience
- **claim_status:** Target variable indicating whether a claim was made (1) or not (0)

## Exploratory Data Analysis

### Distribution of Claim Status

![Distribution of Claim Status](https://github.com/SachiniRathnayake/Insurance-Claim-Prediction/assets/144448061/0e175791-4824-4ad4-96a8-7306ab1e978b)



The data shows a significant imbalance between the classes, with fewer claims (1) compared to no claims (0).

## Handling Class Imbalance

We use oversampling to balance the classes and ensure the model does not become biased toward predicting the majority class.

## Feature Selection

Using a Random Forest model, we identify the top 10 most important features for predicting insurance claims.

## Model Training

A Random Forest classifier is trained on the oversampled data. The model achieves high precision, recall, and F1-score on both classes.

## Results

The model performs exceptionally well, with an overall accuracy of 99%. Here are some key metrics:

- **Precision:** 0.96 (claim), 1.00 (no claim)
- **Recall:** 1.00 (claim), 0.96 (no claim)
- **F1-score:** 0.98 for both classes

## Conclusion

This project demonstrates the effectiveness of handling class imbalance and building a robust predictive model for insurance claims.

