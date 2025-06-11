# Today's Learnings

Like I discussed yesterday about how balancing variance and bias both can increase the performance of the model. Today I'm going to learn some techniques which helps to do it.
Regularization is the name the term which usually used to reduce the overfitting in model, let's go deep into it.

## Regularization

It's a technique which is used to decrease the overfitting in ML model by adding some extra data.

### Techniques

1. Ridge (L2)
2. Lasso (L1)
3. ElasticNet

## Intuition
Let's assume we are working with Linear Regression model.  
We know, overfitting is directly dependent upon the slope value (m).  

Usually, (without regularization)  
L = ∑(y_i - Y_i)^2

In regularization,  
L = ∑(y_i - Y_i)^2 + λ(m^2)  

y_i --> actual value  
Y_i --> Predicted value  
λ --> regularization hyperparameter  
m --> slope

**Due to the addition of extra term loss decreases and overfitting is prevented**
