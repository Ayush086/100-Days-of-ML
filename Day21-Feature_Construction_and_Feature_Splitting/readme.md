# Today's Learnings
*While digging more dip into understanding importance got tackled with constructing new features from existing ones.*
## Feature Construction
Typically means creating new features based on the given data. It's a manual process we need to develop a logic between multiple features to create new one without loosing it's essence.

eg. Dataset have cols: first_name | last_name then we can merge them into one and form new col of "full_name".

**It's not that easy as it seems**

## Feature Splitting 
Rarely used when there is need to split the single col into muliple for better understanding.

 eg. col with seat no. of passengers which contains both numbers + alphabets (like G18) here, G shows the coach no. and 18 is the seat no. But it'll be hard for model to interpret it's importance. Therefore, in such cases feature splitting plays an important role


 ***NOTE: Feature Construction is an very important concept used widely in datasets containing high dimensionality***
