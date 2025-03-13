# Today's Learnings
Deep dived into the maths of Ordinary Least Score (OLS) method. How it's implemented and calculated in backend. It's quiet amazing
to know the implementation part because you will know how the model working which will make it easier for you to reason the bugs or errors you may face.
After getting to know about the maths behind you will be able to determine whether the provided data is perfect to work with that algorithm or not.

## Maths Behind
**How are they(m,c) formulated ?**
We know that,  
&ensp; Best Fit Line (BFL), is the line which pass through/closely from all data points.  
i.e., End goal is **Dist(x, line)** must be minimized.

Assume we have n-points and (d1, d2, ...., dn) are the dist(x_i, line) rply.  
Therefore,``` Error(E) = d1 + d2 + d3 + .... + dn```  
It may be possible that d_i is negative and we are trying to concentrate on magnitude only. That's why we are going to square it up.

```E = d1^2 + d2^2 + ... + dn^2```  
&ensp;&ensp; ```**E = Σd_i**```  -- *Loss Function (J) / Error Function*

So, now we need to find such value of ```m``` and ```c``` which will be used to minimize E.

since,  
&ensp; ```D_i = Y_i - ŷ_i```  { actual_distance - predicted_distance }  

therefore,  
&ensp; ```**E = Σ(Y_i - ŷ_i)^2**```  
After reframing equation,  
##### ```E = Σ(Y_i - mx_i - b)^2``` -- Final Equation

Above equation is totally dependent on ```m``` and ```b``` only.

*Just for better understanding, Remember that ```m``` is responsible for the orientation of line and ```b``` is responsible for the position of line w.r.t to x-axis.*

Since, at maxima and minima any which is differentiable has their 1st order derivative equals to 0.
So, to minimize the error we are going to find partial differentiation of E at 2 cases
##### 1. While ```m``` is constant
After performing partial differentiation on Final Equation. we get,
&ensp;&ensp;```**b = Y_bar - mX_bar**``` -- eqn-1

; ```y_bar = (Σy_i) / n``` & ```x_bar = (Σx_i) / n```

##### 2. While ```b``` is constant
After performing partial differentiation on Final Equation. we get,
&ensp;&ensp;```**m = Σ {(y_i - Y_bar)(x_i - X_bar) / Σ(x_i - X_bar)^2}**``` -- eqn-2


Finally, we got the values to calculate ```m``` and ```b```.

## Assumptions in Linear Regression
**1. Data has Linear Relationship**
**2. No Multicolinearity**
   -  It means if there exist multiple input features but all are independent of each other
**3. Normal Residual**
   - Data is normally distributed, else LR will not work
**4. Homoscedasticity**
   - if we plot a scatter-plot of residuals then it will be uniform about the X-axis throughout the spread.

### It's Important to NOTE that if any of the above assumption isn't satisfied then Linear Regression will not work on that dataset

***I have attached the ![python notebook](./code-from-scratch.ipynb) in which I have implemented OLS method from scratch***
