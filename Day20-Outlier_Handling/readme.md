# Today's Learnings
*What if  data has exception value in dataset ever thought how are they handled and what's their impact on model ?*
## Outlier
**Data points which don't follow the patterns of data points which are followed by majority points.**  
eg. silent boy in class who doesn't talk much with anyone just busy in his own world.  

In above example, the boy is part of class but he doesn't have same behavior (pattern) like others.
Therefore, he will be act as a outlier who has different interests than other students.

![image](https://github.com/user-attachments/assets/8d01b14e-27a5-4cf8-b997-562cb73e1a1d)


Generally they are ignored in datasets because of it's negligible impact on model.
**But sometimes when each and every data point matters (eg. healthcare domain) they are analyzed properly.**

### Impact
In Deep Learning, outliers plays an important role they're not neglected. Whereas in case of Decision Tree not much importance is given to outliers.

### How to handle ?
#### 1. Trimming  
  - Completely removing the data point (row) from the dataset.
#### 2. Capping
- By limiting the value's acceptance range
eg. if range = [A, B] => values less than A or greater than B will be neglected
#### 3. Treat like a missing value
#### 4. Discretization
- By creating bins (clusters/groups)

***In many cases Trimming or Capping is only used.***

### Outlier Detection
#### 1. Normally Distributed Data
In mathematics, if data is normally distributed then 99% of data lies around it's mean within a range of 3 times the standard deviation. (as shown in below image)

![image](https://github.com/user-attachments/assets/f3ef6413-3875-42bb-b627-bf38809d7900)

**z-score method is used to remove outliers from data**  

#### 2. Skewed Distributed Data  
Data points are not symmetrically distributed around mean. Instead they tend to cluster more on one side of mean. (Left-Skewed/Right-Skewed).

![image](https://github.com/user-attachments/assets/719b56f8-4712-496a-b587-4124a7ed78d4)

**IQR method is used to handle removal of outliers in such cases**


