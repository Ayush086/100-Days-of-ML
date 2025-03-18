# Today's Learnings
I learnt about one of the best topic in Machine Learning, Principal Component Analysis (PCA). It's feature extraction method which is widely used for dimensionality reduction.


Yesterday I learnt about curse of dimensionality, how does it affects the model's performance, why there is a need to prevent it. Today I explored a method to prevent it.
## Feature Extraction
It's one of the technique which is used to reduce the dimensions of the dataset. There are multiple methods which are used to perform feature extraction and PCA is one of them.

### Principle Component Analysis (PCA)
In general words, PCA is used to bring higher dimensional data to best possible lower dimensional data.

Let's understand it with an example,  
Assume you are watching a cricket match and you click a photo of players playing to capture the moment.  
Now, Players are playing in 3D world and after clicking photo you have captured the photo in 2D image.  
Therefore, you converted 3D (cricket moment) to 2D (photo). Obviously, there is no use of PCA in here but to understand the essence we can think of it likewise.

#### Why to use PCA ?
##### 1. Dimensionality Reduction
- Lower dimensioned data is cheaper to compute and it's easier for ML algos to find complex patterns/relations from data.
- Lower the dimensions => higher will be the throughput + performance.

##### 2. Data Visualization
- Since, we can't visualize data with more than 3 dimensions. So PCA is used to visulize those datasets to draw the observations and to analyze the distribution of datasets.
- N-D datasets are converted to 3D/2D graphs to visualize them.

Now, I have gained the usage of PCA and it's importance in ML. But in real how does it works ?, How does it converts the data in lower dimensions ?. Tomorrow I'll learn about the working of PCA and Mathematics behind it.



***Keep Grinding***
