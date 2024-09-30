# Today's Learnings
***I learned about Feature Engineering***
## Feature Engineering
It's the process of using domain knowledge to extract features from raw data.
- i.e., Raw Data ---> ML Algorithm Consumable data

### Feature Transformation
- Datatype Conversion (from one form to another form).
- Generally, missing values handling, categorical features handling is performed.
- Also feature scaling and outlier detection is performed.
- e.g. In a cars dataset, kms_traveled feature is of type 'string', need to convert it to 'int' for model training.

### Feature Construction
- Creating/Developing new feature using existing features
- Adding data which isn't directly available in data.
- e.g. We have a dataset in which height, weight is given calculating BMI on the basis of it.

### Feature Selection
- Irrelevant features are present in dataset which aren't required during model development.
- Multiple similar features are present only relevant must be extracted.
- Performed using random forest, etc.

### Feature Extraction
- Developing new features from existing but programmatically.
- Mainly used to reduce dimensionality of data by transforming it into new feature space.
- Algorithms like PCA, LDA are used to reduce dimensions of the data.
