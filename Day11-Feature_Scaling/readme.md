# Today's Learning
***As I dug more into the feature engineering I got introduced with feature scaling. Today I got to understand about why their is a need of feature scaling in ML and before that 
what is feature scaling ?***

## Feature Scaling
It is a technique which is used to standardize the independent features present in the data in a fixed range. In simple words, scaling down the values in ranges or by changing the units.

After reading definitions I understood what does it mean but I was thinking why do we need it, what's it's use ?. Let's explore it !


#### Why do we need Feature Scaling ?
- If you know there are many alogrithms which uses distance between the points to predict.
- e.g. KNN (Kth nearest neighbour)
- *It basically finds the similar record within dataset and the returns the output of most similar data point from the dataset*
- For example, I'm trying to build a model which will find the breed of a dog from it's appearence properties. So here I will use KNN Algorithm and my dataset will contain all the required properties of dogs to distinguish
  between them. The more the properties I will give to my model the more will be the accuracy of my model of finding the dog's breed.

- Another reason why scaling is needed is that computation time decreases if the values involved are small. If small range of values then faster will be the calculation of operations performed.

### Types
1. Standardization
2. Normalization
