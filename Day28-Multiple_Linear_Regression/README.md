# Today's Learnings
After gaining the knowledge about simple linear regression, now I'm heading towards the multiple regression to explore more advanced version of linear regression.

## Multiple Linear Regression
Unline Simple LR where i/p must be a single element, here in this case i/p can have multiple values and o/p will be single value. It's nothing but the extension of Simple LR to 
handle more complex/n-dimensioned data.

### Mathematical Intuition
In Simple LR,  
&ensp;&ensp; ```y = mx + c```

In Multiple LR,  
&ensp;&ensp; 
![Screenshot 2025-03-17 172505](https://github.com/user-attachments/assets/31bb742a-0844-4d01-bcb8-254cc1ad09ea)  
where,
&ensp; 𝛽o - intercept (offset)  
&ensp; 𝛽1, 𝛽2,..., 𝛽n - weights of feature to calc. y (dependency factor)  
&ensp; x1, x2,..., xn - independent variables (input)   

**In case of multiple LR, Loss Function changes which involves lot more variables when compared to simple LR.**  

If we use OLS in multiple LR complexity grows to O(n^3) that's why we use *Gradient Descent*.
I'm going to learn about it tomorrow.


Also attached a python notebook in which I tried experimenting with multiple linear regression.
