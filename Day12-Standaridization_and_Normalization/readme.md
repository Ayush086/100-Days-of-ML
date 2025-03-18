# Today's Learnings
***Today I dug more into feature scaling and it's types***
## 1. Standardization
Technique used to scale values after which features becomes comparable after scaling.

It uses z-score normalization technique for scaling values.

![formula](https://github.com/user-attachments/assets/9785276a-04f5-4618-94d3-14855d47a0c8)

- Mainly **Mean Centering** method is used in standardization
- In Mean Centering, mean = 0 and st. deviation = 1 is considered.

**When to use it ?**
While using following ML algorithms:
- K-Means
- KNN
Can also used for implementing these techniques, PCA, ANN, Gradient Descent, etc.

**What if outliers are present ?**
- Outliers impact doesn't get affected after implementing standardization.

  **NOTE: Before scaling the values always perform train_test_split on data for smooth performance**
  
## 2. Normalization
- This technique is used to change the values of numeric columns in dataset to use a common scale without distorting difference in ranges of values or losing info.
- eg. preventing the use of units.
- Outliers will get affected in this method.


  
### Types
#### MinMax Scaling
- Values will be scaled in range of [0-1]

Xi'= (Xi - X_min) / (X_max - X_min)

#### Mean Normalization
- Used when centered data is needed.
  
Xi'= (Xi - X_bar) / (X_max - X_min)

#### MaxAbs Scaling
- Used when sparsed data is present.
- Sparse matrix is constructed.
