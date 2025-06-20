# Today's Learnings
Got introduced with one of the technique of regularization, Ridge Regression. Let's see what and how does it minimises loss in a model.

## Ridge Regression 

- Also called as L2-regularization.
- As discussed yesterday, due to the addition of an extra term (λm^2) overall dependence upon m-value decreases.

### Mathematical Intuition
#### 1. Using Ordinary Least Score (OLS) method:

After addition of extra term,  
 ```L = ∑(y_i - Y_i)^2 + λm^2```            &emsp;&emsp;  &emsp;                    here: y_i - actual values; Y_i - predicted values

 Now we need follow the same process which was performed during linear regression, derivating w.r.t. ```m``` and ```b``` equals 0.  
 After applying partial derivation we get,  
 ```b = y_bar - mx_bar``` &  
 ```m = {∑[(y_i - y_bar)(x_i - x_bar)]} / {λ + ∑(x_i - x_bar)}```

 As we can see ```b``` is same as in linear regression but value of ```m``` has extra term in denominator ie., ```λ```

 ***This extra term in denominator affects the result of loss function as the ```λ``` value increases the ```m``` will decrease.***

 **In N-dim data**,  
 extra term will be ```λ||w||^2``` 

 ### Key Understandings
 1. As value of coeff increases ```m``` shrink towards 0.
 2. More the value of coeff more will be the impact of ```λ```.
 3. As we increases value of ```λ``` overfitting reduces but if we increase it much more model will start to underfit the data.


***NOTE: Use ridge while dealing with more than 2 i/p parameters.***
