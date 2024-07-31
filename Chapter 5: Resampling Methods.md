# Chapter 5. Resampling Methods

Resampling approaches can be computationally expensive, because they involve ftting the same statistical method multiple times using different subsets of the training data.

Resampling methods involve repeatedly drawing samples from a training set and fitting a model of interest on each sample in order to obtain additional information about the fitted model.

## Two main resampling methods: Cross-Validation and the Bootstrap.

### Introduction

The process of evaluating a model’s performance is known as model assessment, whereas the process of selecting the proper level of flexibility for a model is known as model selection.

### Bootstrap Intro.

-most commonly to provide a measure of accuracy of a parameter estimate or of a given statistical learning method.

## Cross-Validation
-The training error rate often is quite different from the test error rate, and in particular the former can dramatically underestimate the latter.
-The validation set approach, is a very simple strategy for this task. It involves randomly dividing the available set of observations into two parts, a training set and a validation set(hold-out set).
-The validation set model is fit on the training set, and the fitted model is used to predict the responses for the observations in the validation set.
-The results of validation set error rate - typically like MSE – provides an estimate of the test error rate.

![image](https://github.com/user-attachments/assets/c4b6f326-4801-4e15-9eb3-0f49a063915f)

![image](https://github.com/user-attachments/assets/64651289-1240-4e23-b155-a6b4b5ec8efd)


### Leave-one-out cross-validation (LOOCV)
A single subset of training set is used for validation set, and then train. 

This is done repetitively until each single subset from training set is used for validation Set to train the remaining data to get every training error rate.

![image](https://github.com/user-attachments/assets/a1cf9b81-f4be-44c6-86d1-4720fbe58611)

#### Advantages of LOOCV

1. Less bias

2. Always yield the same results since there is no randomness

#### Disadvantages of LOOCV

- Too much time consuming -> SLOW!

->Alternative method: k-fold Cross-validation.

### K-fold Cross-Validation
-Involves randomly dividing the set of observations into k groups, or folds, of approximately equal size.

![image](https://github.com/user-attachments/assets/f9ae2ca9-92de-4be8-a7d1-7a19c3fde9b8)

### Why K-Fold Cross-Validation??
-Less computer cost than LOOCV, and less randomness than ordinary Cross-Validation methods.

## Bootstrap
-A resampling method that estimate the value of a parameter that minimizes the variance of our investment using simulations over the data and then use standard deviation of the parameter's estimation over and over.

-Allows us to use a computer to emulate the process of obtaining new sample sets, so that we can estimate the variability of the estimator without generating additional samples.

### Bootstrap Summary
-We instead obtain distinct data sets by repeatedly sampling observations from the original data set.
