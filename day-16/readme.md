# Today's Learnings
**Learned about Mathematical Transformation and it's uses types**
## Mathematical Transformation
- *It is a part of feature tranformation in which transformation is performed using mathematical formulas and relation.*  
- After applying this tranformations techniques, features following Probability Density Function (PDF) with convert into Normal Distribution (ND).

### Types
- Log Transform
- Reciprocal Transform
- Power Transform
- Box-Cox Transform
- Yeo-Johnson Transform
- Quantile Transform

**Might be thinking why do we use them ?**  
In Statistics, Normally distributed data makes calculation easiear and many Machine Learning models perform well on normally distributed data.

#### Always Remember
***If you're working with maths related algorithms (eg. linear regression, etc) then they need data which is normally distributed else they won't perform well and results will be reliable.***

**How will I know if data is normally distributed or not ?**
- Using plots mainly sns.displot
- Check pd.skew() if 0 returned that means data is normally distributed.
- Most reliable method is using **QQ plots**.


### Function Transformer
#### 1. Log Transform (log(x+1))
- Takes log of each value with base 2/10.
- Mainly used when data is right-skewed.
- makes data more normally distributed if compared to data without any transformation.

#### 2. Reciprocal Transform (1/x)
- Not used on large scale.
- Just changes the skewness direction
- badi values choti ho jaati hai and choti values badi.

#### 3. Square/Square root Transform (X^2 / X^1/2)
- X^2 Transform is mainly used for left skewed data.
- sq. root transform is not used widely.
