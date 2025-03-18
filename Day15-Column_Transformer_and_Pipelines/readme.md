# Today's Learnings
***I learned about column transformers and pipelines in machine learning***

## Column Transformer
Let's understand it with an example,  
we have a dataset with headers, **Age | City | Gender | Review**  
- 'age' column may have missing values so we can perform simple imputation to fill them.
- 'city' and 'gender' col will contain categorical/string values which need to be converted to numerical using one hot encoding (OHE). since, it's relative order isn't important that's why we are using OHE.
- 'review' will have categorical values so here we can apply ordinal encoding (OE) since order matters here.

If we perform this 3 steps separately then it will create 3 different outputs and them mergin them into one dataframe makes this process inefficient.
**Column Transformer** performs all the 3 steps in one go and merges dataframes on their own.

***NOTE: Attached a python notebook (Column_Transformer.ipynb}) implementing same thing with and without using column transformer for better understanding.***


## Pipelines
It chains together multiple steps so that output of each step is used as input to next step.

Let's understand with practical case,  
In Data Preprocessing, we perform various steps like:  
- adjust missing values
- convert categorical data to numerical
- scaling
- prediction  
*taking rough case*  

Usually we perform each step separately but by using pipeline we can create a transformer of each step and can use it like a variable anywhere we want in our project.

At production level also every time we don't need to preprocess data, it automatically gets converted into required form and shows us the results with the help of pipeline.


### Difference between Column Transformer and Pipelines
**Column Transformer** is used for handling different tranformations on different columns whereas **Pipelines** are used to handle preprocessing workflows.  
eg.: column tranformer: handling missing data, datatype conversion but pipeline: data transformation + model training + testing + prediction.

**NOTE: Attached a folder (pipeline) containing a practical implementation of model training with and without using pipelines.**
