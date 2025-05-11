# Today's Learnings
Explored an interesting concept which is mostly used in Deep Learning but can be learnt in ML. Previously I explored concepts of stochastic and batch gradient descent. This is the
combined version of both i.e., mini-batch GD.

## Mini-Batch Gradient Descent
Generally used in DL.  
As we know,  
In Batch GD --> 1 update/epoch, it's feasible with small dataset with convex function (i.e., single minima/maxima).  
In Stochastic GD --> N-updates/epoch, it's feasible with larger dataset with non-convex function (i.e., multiple local and single global maxima/minima).  


Therefore in Mini-Batch GD,  
Batch = group of n-rows  
batch_size is decided by user  

So,  
if batch_size = 1 --> Batch GD  
if batch_size = N --> Stochastic GD
