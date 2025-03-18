# Today's Learnings
Actually I was going to start multiple linear regression but then yesterday when i was building my first ever model (simple LR), i missed to calculate it's accuracy then I remembered 
than I have not learnt about the evaluation metrics in ML. So today I decided to understand them and then we'll jump onto next algorithm.

## Regression Metrics (Evaluation Metrics)
This metrics are used to determine model's efficiency, based on the result of this metrics we decide whether model is performing well or not ?. So let's dig into it.
### 1. Mean Absolute Error (MAE)
As name suggests it's the mean of absolute errors of each point in dataset.  
![image](https://github.com/user-attachments/assets/d74ab159-fe2a-4472-b0e5-4a2780ba4e99)

It's very useful in outlier handling but it's not differentiable at 0 that's why not considered many times.

### 2. Mean Squared Error (MSE)
Better version of MAE, instead of taking absolute error we take square of error to make it differentiable at 0.  
![image](https://github.com/user-attachments/assets/fb47d748-a056-4802-9e8d-899da2240cca)

But it lacks outliear handling and o/p's unit isn't same as i/p.

### 3. Root Mean Squared Error (RMSE)
It's the root of MSE, it just that output's unit will be same as of input.  
![image](https://github.com/user-attachments/assets/7fd0dad3-cf70-4a3f-af2c-6f828289f6bc)

It also lacks outlier handling.

Above all metrics have their own advantage and disadvantage and they are context dependent, means they can't used everywhere because:

1. **Treatment of Errors**:
   - **MAE**: All errors are treated equally.
   - **MSE**: Penalizes larger errors more (squares errors).
   - **RMSE**: Similar to MSE but in the same units as original data.

2. **Application**:
   - **MAE**: Useful when all errors have equal importance.
   - **MSE/RMSE**: Suitable when larger errors are critical to minimize.

3. **Sensitivity to Outliers**:
   - **MAE**: More robust to outliers.
   - **MSE/RMSE**: Can be heavily influenced by outliers.

4. **Interpretability**:
   - **MAE**: Intuitive and easy to understand.
   - **RMSE**: Directly comparable to data scale.
***Therefore, not every time we use this metrics, there is one more technique which is used for every model evaluation.***

### 4. R2 Score
Also called as *coefficient of determination*. It's the comparison between regression line and mean line.  
R2 = 1 – (RSS/TSS)

Where,  
R2 represents the requrired R Squared value,  
RSS represents the residual sum of squares, and  
TSS represents the total sum of squares.  


![image](https://github.com/user-attachments/assets/7afdbe17-a5f0-4c3d-abe1-bf414480660c)


R2 = 0 --> Not well  
R2 = 1 --> Perfect  
R2 < 0 --> Worst

eg. R2 = 0.8 it means x_i explains 80% variance of y_i values. 
