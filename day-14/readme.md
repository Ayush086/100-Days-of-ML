# Today's Learnings
***I discovered a small concept of Dummy Variable Trap**
## Dummy Variable Trap
It's very small concept but it's very important many people don't recall it when they are asked about it.  

In One Hot Encoding (OHE), we need to remove any one col from all newly generated columns (generally 1st col).  
Let's say if there are n-categories,    
&nbsp; therefore, n columns will be generated 
&emsp;  then consider n-1 values only drop anyone column.

**Why do we do it ?**
It's to prevent multicollinearity

**What is Multicollinearity ?**
Let's understand it with an example,  
Multicollinearity occurs when two or more independent features in a regression model are highly correlated with each other. This means that when one variable changes, it can predict changes in another variable quite accurately. For example, if you have features like "height" and "weight," they may be correlated because taller people often weigh more.
Why is it a Problem?
Difficult Interpretation: In a regression model, we want to understand how each feature affects the outcome. When features are correlated, it becomes hard to isolate their individual effects. For instance, if both height and weight are used to predict health outcomes, it’s challenging to determine which one is more influential.
Unstable Coefficients: Multicollinearity can lead to large standard errors for the coefficients of the correlated variables. This means that small changes in the data can lead to large changes in the estimated coefficients, making the model unreliable.
Overfitting: Models with multicollinearity may fit the training data very well but perform poorly on unseen data because they are too complex and sensitive to noise in the training data.
