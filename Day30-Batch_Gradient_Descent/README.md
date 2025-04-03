# Today's Learnings
Digged more deep into the world of gradient descent. Today I explored the concept of Batch Gradient Descent.

## Batch Gradient Descent
Till now to calculate the value of (m, b) we were taking random values of m & b to start with and then updating to get the best fit values.
But in Batch GD, We calculate slope of every point like we used to do before.

*Let's understand this with an example*,  
Assume ```y = b0 + b1x1 + b2x2 ```,   
S1: start with random values. (Generally b0=0, b1,b2=1)  
```b0 = 0; b1,b2 = 1```

S2: Decide epochs and learning rate value.  
Epoch = 100; lr = 0.1  
Therefore,  
```b0 = b0 - lr*(slope of b0)```  
```b1 = b1 - lr*(slope of b1)```  
```b2 = b2 - lr*(slope of b2)```  

Now, imagine how much computation will it need to find the equations for each derivative and then calculating them at epoch iteration in epochs.  
**Sounds Like a Tough Work**  
and yes, you're correct!

Here, we need to calculate the derivative for each b-value we need to find n-tems derivative. (n -> no. of features)  
e.g., rows = 1000, epoch = 50, features = 5 --> 6-coeffients   
in each epoch  
&nbsp; 1 - coeff will need 1000 derivatives  
similary,  
&nbsp; 6 - coeffs will need 6000 derivatives

for 50 epochs it will need (50 x 6000) derivatives.

That's why,  
***Batch GD is not preferred in ML, Also not in DL. In DL, we mainly deal with large datasets with high dimensions so Stochastic GD is mostly used***.
