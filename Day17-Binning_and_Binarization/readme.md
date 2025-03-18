# Today's Learnings
*Usually we prefer to have numerical data in our dataset. But sometimes we get more efficiency by using categorical data.*

**Might be thinking how and why ?**  
 Since we've learned that numerical data is processed faster and makes algorithms to understand data in better way.

Let's understand this with an example,  
	- Assume we have a dataset of apps downloads on play store.  
	- Now instead of showing the exact count we show it in terms of K, M, T, etc.    
	- By creating categories we are making it more feasible for our model to understand it better.  
	
## Encoding Numerical Features
There are mainly 2 methods which are used for the conversion.
### 1. Binning (Discretization)
*It's the process of transforming continuous variables into discrete variables by creating a set of contiguous intervals (called as **Bins**).*  
**Why do we use it ?**  
	- Efficient outlier handling.  
	- Improves value spread by making bins and also uniforms the data spread.  
	
It's dividing into 3 categories  
1. Unsupervised  
	- Uniform Binning - equal width  
	- Quantile Binning - equal frequency  
	-  K-means  
2. Supervised    
	-  Decision Tree Binning   
3. Custom Binning  

Let's understand each category separately  
#### Uniform Binning  
Equal sized bins are created based on the input of bins count.  
	**bins = ( max_value - min_value ) / bins_count***  
There is no change in data spread but outliers are handled well.  

#### Quantile Binning    
Bins will be created on the basis of frequency count.   
eg. if bins_count = 10  
therefore, each interval will have 10% each observation  
I1 - 0%ile to 10th%ile   
I2 - 10th%ile to 20th%ile and so on.  

Here interval width may vary but the frequency count will be same.  

#### K-means Binning
It's an clustering algorithm which can form clusters in any dimension.

#### Custom/Domain Based binning
Creating bins by on our own


### 2. Binarization
*It's the process of converting continuously distributed into discrete distributed data.*
Mostly used for boolean type data.
eg. if(salary > 60K) return true
      else return false

***NOTE: All the implementation related to it is attached in python notebook.***
