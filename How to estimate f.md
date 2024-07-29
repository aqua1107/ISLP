## How to estimate $f$?

### Keypoint: Use observations, so called training data to TEACH A METHOD TO ESTIMATE $\hat {f}$. This is our goal.

### Two Methods: Parametric Methods and Non-parametric methods

### Parametric Methods

1.  Make an assumption about the functional form, or shape, of $f$.

2.  Need a procedure that uses the training data to fit or train the model, after selecting a model.

#### Summary

Model-based approach can be said as Parametric Methods.

##### Advantages

- Reduces the number of parameters to estimate $f$. => easier to estimate a set of parameters.

##### Disadvantages

-  The model we choose will usually not match the true unknown form of $f$.

-  Alternatives: Use flexible models that can fit many different possible functional forms flexible for $f$. But it requires more parameters, causing *overfitting the data. 

-  *Overfitting: Follow the errors too closely.

### Non-Parametric Methods

- Seek an estimate of $f$ that gets as close to the data points as possible.

##### Advantages

- Have a potential to fit possible shape of $f$ more accurately.

##### Disadvantages

- Need big data to accurately estimate $f$.
