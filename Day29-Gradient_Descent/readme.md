# Today's Learnings
*Today I learned about one of the interesting and very important topic. An optimization technique used widely, Gradient Descent.*

## Gradient Descent
It's used to find local minima of a differentiable function. Unlike OLS, it's not calculated using a single formula. Uses basic learning method find the minima.
Many says it's the backbone of Deep Learning.

## Intuition
Imagine you're standing on a hilly terrain in the dark, and you want to find the lowest point (the valley). Without being able to see, you take small 
steps downhill based on the steepness of the slope at your current position. This process of taking steps downhill is analogous to gradient descent.


**Objective:** Minimize a loss function.

**Gradient Calculation:** The gradient represents the slope of the loss function at a particular point. It tells us the direction in which the function increases the most.

**Update Rule:** Take a step in the opposite direction of the gradient (downhill), adjusting the parameters of the model iteratively.
  - The size of each step is controlled by a parameter called the learning rate.

**Iteration:** Repeat this process until you reach a minimum (ideally the global minimum, but sometimes a local one).

## Types
1. **Batch Gradient Descent:** Uses the entire dataset to compute the gradient. Slower but stable.

2. **Stochastic Gradient Descent (SGD):** Uses a single data point for each update. Faster but noisier.

3. **Mini-batch Gradient Descent:** A hybrid approach that uses small batches of data, balancing speed and stability.

Actually I digged more into maths behind it but it's not possible to explain it here. Tomorrow I'll explore each type of GD in detail.
