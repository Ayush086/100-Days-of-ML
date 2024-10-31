# Today's Learnings
*Ever thought how data with missing values are treated are they dumped or missing values are filled with dummy values ?*

## Missing Values Imputation
### 1. Univariate Imputation
**To fill up the missing values we take help other present values of same column.**
eg. mean, median, mode, etc.

#### Methods
###### Mean/Median
This is the goto technique when it comes to missing value handling.  
But it affects the data distribution which results in change in covariance.
*Covariance describes the correlation/dependency of a column with other columns.*

###### Arbitrary Value (random value)
mainly used for categorical data

##### End of Distribution
- Extension of Arbitrary Value just with a small change that values are selected from the end of distribution of data. (limiting values)
- Maintains the distribution's behavior.

##### Categorical Missing Data
- Usually missing values are filled with most frequent data.
- In rare cases, new category **missing** is created for missing values.

### Multivariate Imputation
**We take help of other feature's values of same row to fill up the missing space.**
eg. finding another row same values of other features and replacing missing value with the value present in other row data.  

***There are many Imputers which are widely used to handling missing data.***
