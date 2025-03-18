# Today's Learnings
From today onwards I'm starting to learn about each algorithm or technique in machine learning. My first algorithm will be *Simple Linear Regression*.

## Linear Regression
It's a supervised ML algorithm. Usually categorised into 4 types:
**1. Simple LR** - 1 i/p --> 1 o/p
**2. Multiple LR** - 1+ i/p --> 1 o/p
**3. Polynomial LR** - handles non-linear relationships
**4. Regularization Methods** - used to reduce overfitting


## Simple Linear Regression
Very simple algorithm. In simple words, it's an compare and answer algorithm.

![image](https://github.com/user-attachments/assets/11be0b8d-6c61-4707-9846-4cbdd1c17329)

As we can see in above image,   
    Line going through points is called as best fit line (regression line). It's the line which is closest to all points in dataset when they are plotted on 2D plane.

### Mathematical Intuition
Mathematially, Best fit line can be represented as:   
## &ensp;&ensp;&ensp; y = mx + c

Here, model's work is to find value of **m** and **c** such that the line is closest all the points in scatter plot.

***In ML, there are multiple ways to find out the value of ```m``` and ```c```. It totally depends on the data and problem statement which method to choose.***  
### Methods
#### 1. Closed Form
- Using Quadratic Equation Formula:  
  &ensp; x = (-b ± √(b² - 4ac)) / 2a
  
- Ordinary Least Score (OLS):
  &ensp; This method is implemented in scikit-learn library.

#### 2. Non-Closed Form
- Gradient Descent:
   Usually used when dealing with complex data and commonly used in deep learning models. In higher dimensioned data OLS method doesn't work.


***Attached a [python notebook](./simple-linear-regression.ipynb) where i have trained a basic LR model.***
