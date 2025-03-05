# Today's Learnings
Deep dived into the implementation of PCA, understood how it reduces the dimensions what's logic behind and what are the more usage of it in industry.

## Intuition Behind It
Let's understand it with an example,  
Assume you have a dataset --> # rooms | # grocery_shops_nearby | flat_price

Now with if I say you have to develop a model to predict ```flat_price``` based on given data then you'll say that col = ```# grocery_shops_nearby``` will not help in predicting the prices.   
**And yes you're correct !**

*In above case we knew which features are important because we had domain knowledge, But what if we get tackled with a dataset of which we have no domain knowledge then above logic will not work.*

In ML, ***Features with more variance must be given more priority***. But not every time we can perform feature selection.

It may occur that you had the dataset in which all the features are important (eg. MNIST dataset). At that time you'll need some approach to handle all features simultaneously.

**PCA is used as a saviour in this cases**.


## Working
1. Existing features ko bhul jayega.
2. With the help of ```Old Features``` it will create ```New Features```.
3. Now after creating ```New Features``` only best fit features will be selected.


Above is the overall logic behind it's working. Let's dive more into it!

## Mathematics Behind
***Variance must be maximised so that relation between data points doesn't get dissolved***.
NOTE: Variance explains the behaviour of data. Variance is nothing but the data spread in a co-ordinate system.

Let's understand this, If we have 2D data and we see the data distribution of data from anyone axis only you'll be able to see the data spread across that axis only. Now, you will prefer to watch the data 
distribution from that side which has more spread to understand it better. That's it.

Therefore, variance is important to find relations between features.

### **1. Covariance Matrix**  
The *covariance matrix* captures the variance and relationships between variables in a dataset. It is symmetric and represented as:  

```
Covariance Matrix =
[ Var(x)   Cov(x, y) ]
[ Cov(y, x)   Var(y) ]
```

- *Diagonal elements*: Variance of individual variables (`Var(x)`, `Var(y)`).  
- *Off-diagonal elements*: Covariance between variables (`Cov(x, y)`). 


#### **Key Notes**:  
- A covariance matrix is always **symmetric**.  
- **Positive covariance** → Variables move in the same direction.  
- **Negative covariance** → Variables move in opposite directions.  

---

### **2. Linear Transformations**  
A *linear transformation* changes the coordinate system (e.g., scaling, rotation). It is defined by a transformation matrix. It's the key step in PCA

#### **Example**:  
For a transformation matrix  

```
M =
[ 1  0 ]
[ 0  1 ]
```

the grid remains unchanged.  

**NOTE: coordinate system is nothing but a linear transformation.**

#### **Key Points**:  
- Matrices represent linear transformations of coordinate systems.  
- Applying a matrix **changes the basis (coordinate system)** while preserving linearity.  
- A *coordinate system* is essentially a collection of vectors.  

---

### **3. Eigenvectors**  
*Eigenvectors* are special vectors that do not change their direction under a linear transformation.  

#### **Example**:  
Given a vector  

```
x =
[ 1 ]
[ 0 ]
```

after applying a transformation  

```
M =
[ 3  0 ]
[ 0  2 ]
```

the transformed vector remains in the same direction.  

#                                    &nbsp;&nbsp;&nbsp;&nbsp;               AV = λv  
where,
  A -> Matrix  
  V -> Eigen Vector  
  λ -> Eigen Value  
  v -> vector

**Eigenvectors help in PCA** because they define the new axes along which the data is projected.  
---

### **Final Thoughts**  
- In PCA, Covariance Matrix is used as a matrix from above relation.  
- Covariance Matrix defines both spread (variance) and orientation (covariance) of the data.  

***Therefore, largest eigen-vectors of covariance matrix always points into the direction of largest variance of data.***


