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

NOTE: Attached a python notebook (Column_Transformer.ipynb) implementing same thing with and without using column transformer for better understanding.
