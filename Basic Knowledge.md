# An Introduction to Statistical Learning with Applications in Python
## Basic Concept
$$Y = f(X) + \epsilon$$

$Y$ : response variable(dependent at  $X$)

$f$ : unknown function of  $X$

$X$ : a collection of feature vectors(predictors). i.e. matrix form

$\epsilon$ : error term with mean 0 and independent from the feature martix  $X$.

Want to predict  $f$ -> WHY?

Why do we estimate  $f$?


-Prediction


-Inference


### Prediction

We do not know the output  $Y$  easily. 

Since the error averages to 0, it seems like we can predict  $Y$  with  $f(X)$  only. 

The ultimate goal is to accurately predict  $Y$  with the estimated function  $\hat {f}$  with the predictors  $X_1$ , ...,  $X_p$, yielding  $X$.

#### Before, we need to know the two kinds of error terms to understand the system of prediction.

##### Reducible error term: Possible to improve the prediction with a more accurate technique. (Therefore, reducing the error)
##### Irreducible error term: Is a function of Y. (Therefore, cannot predict the error. Thus, not reducible)

### Summary

$$E(Y-\hat {Y})^2 = E[f(X)+ε-\hat {f}(X)]^2 = (f(X)-\hat {f}(X))^2 + Var(ε)$$

Expected value :

$$E(Y - \hat {Y})^2$$ 

Reducible error :

$$(f(X)-\hat {f}(X))^2$$ 

Irreducible error :

$$Var(ε)$$

### Inference

Find a relationship between $X_1$, ..., $X_p$ and $Y$.

Need to know its exact form!! But, depending on each individuals, 

the paradigm(whether what variables are more important or not) and model(each combination of variables may vary) of inference changes.
