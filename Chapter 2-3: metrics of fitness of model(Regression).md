### Preface: This is discussing about the evaluation of our model.

## Evaluation of model in regression: Usually MSE!!

## MSE
Definition of MSE given data $x_0$: 

$$E(y_0 - \hat {f}(x_0))^2 = Var(\hat {f}(x_0)) + [Bias(\hat {f}(x_0))]^2 + Var(\epsilon)$$

Expected test MSE:

$$E(y_0 - \hat {f}(x_0))^2$$

### Conclusion

The overall expected test MSE should be the average of expected test MSE for all test data.

### Additional Explanation

Variance: the amount by which $\hat {f}$ would change by estimating with using a different training data set.

Bias:  the error that is introduced by approximating a real-life problem. Extremely complicated.

Use more flexible methods => Variance $\uparrow$ => bias $\downarrow$



### Bias-Variance trade-off in a nutshell


![image](https://github.com/user-attachments/assets/addc8e2e-7121-4e5d-b360-a164d0262a44)
