# Today's Learnings
Explored another type of gradient descent i.e., stochastic gradient descent, which is oftenly used while dealing with large datasets.

## Stochastic Gradient Descent
In Batch GD we used to process whole dataset at every epoch for value calculations but in Stochastic GD we update values after processing each row.

For example we have a dataset consisting 100 rows and doing 10 epochs.
In Batch GD,  
&nbsp; &nbsp; we would have updated variables values after the completion of each epoch.  
which results in relatively slower convergence than Stochastic GD.
Total computations in Batch GD = 10 X 100 = 1000 computations

In Stochastic GD,  
&nbsp; &nbsp; we would update variables values at each row.
which may result in faster convergence towards the desired values
Total computations will be less than 1000 in this case because of frequent updation of values. therefore, not all epochs will be used to find the final results.

*NOTE*: In Stochastic GD, rows are not processed sequentially at every step we randomly select a sample and process to make sure we cover most of the variations from dataset.

### When to use stochastic GD ?
-  when dealing large datasets (for faster convergence).
-  Non-convex function - involves many local minimas and a global minimas
    - due to precence of randomness it may skip local minimas and result in finding in global minima.
 
***REMEMBER: We use learning scheduler with Stochastic GD, it's used to vary the learning rate. Because of it's random nature it may fluctuate form it's
optimal solution so to prevent it learning scheduler is used.***

**Attached python notebooks which contains the implementation of SGD**
