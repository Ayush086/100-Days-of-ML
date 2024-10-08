# Today's Learnings
***I learned one more technique which makes data more machine understandable. Mainly used for categorical data***
## Feature Transformation
Used for encoding categorical variables.  

**Why do we perform this technique ?**  
Because ML algorithms doesn't accept strings as input format many times.

Let's start from basics,  
Categorical data are divided into 2 categories:
  - Nominal: Each value is considered
    - eg.: branch in college
  - Ordinal: Range based data
    - eg.: grade distinction (1st class, 2nd class, etc)
   
### Ordinal Encoding
- In this case ordering matters. Assigns the code to categorical data based on it's relative order.
- eg.: person's education {HS(1) -> UG(2) -> PG(3)}
- Encoded values reflects the actual ranking.

#### There are 2 methods to encode Nominal Categorical Data
As in this case relative ordering doesn't matters.
### 1. One Hot Encoding (OHE)
- For each unique category it creates a new column
- present data is marked as 1 and others are marked as 0.
- It's like a binary variable
- eg.: colors: red, blue, green then each color will have it's own column **red | blue | green** containing 0s and 1s, then they're put together like in array and treated as vectors.
- It increases dimensionality but categories can be classified independently.

### 2. Label Encoder
- Each unique category will have unique integer associated with it and then category value will be replaced with integer value which was mapped to it.
- Usually integers mapped on the basis of alphabetical order or it's frequency.
- eg.: colors: red, blue, green converted to 1, 2, 3.
- It may create confusions for ML alogorithm, usually they try to find patterns between them which may affect the performance and results.

**NOTE: It's totally dependent on scenarion which encoding algorithm to use, you need to try out each one of the independently and compare the results and then move ahead**
