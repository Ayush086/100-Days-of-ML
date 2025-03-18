# Today's Learnings
*One of the best and important concept in machine learning, **Curse of Dimensionality (COD)***

## Curse of Dimensionality
In ML, if more than required features are present in our dataset then model will underperform. Every algorithm
has it's own feature count for an optimal solution.

Let's understand this concept with an example,  
Imagine you are trying to analyze the performance of cricket players to predict their future performance and help in team selection.  
Initially, you start with a few basic features:  
Feature-1: Batting Average  
Feature-2: Bowling Average  

With just these two features, it's relatively easy to analyze and compare player performances. You can identify patterns and make decisions based on these metrics.  


Now, to improve the analysis and make more informed decisions, you decide to add more features:  
Feature-3: Strike Rate (batting)  
Feature-4: Economy Rate (bowling)  
Feature-5: Number of Centuries  
Feature-6: Number of Wickets  
Feature-7: Fielding Percentage
...and many more, until you have 50+ features.

As the number of features increases, the data becomes more complex, and the high-dimensional space makes it difficult to find meaningful patterns. The "distance" between player performances in this high-dimensional space starts to lose its significance, and the analysis struggles to differentiate between good and bad performers accurately.

**Remember**, *Usually COD is seen in case of Higher Dimensional Data.*  

#### You might be thinking then how to handle large datasets ?
## Solution -> Dimensionality Reduction
### Dimensionality Reduction
It means reducing the number of features in dataset.  
We have 2 methods to do so:  
#### 1. Feature Selection:  
  - select the subset of features which are more important and contribute more in model's performance.
  - Methods: Forward Selection, Backword Elimination
#### 2. Feature Extraction:
  - creating new features from existing one and using them instead of previous features.
  - Methods: PCA, LDA
