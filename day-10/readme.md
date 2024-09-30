# Today's Learnings
***I learned about Feature Engineering***
## Feature Engineering
It's the process of using domain knowledge to extract features from raw data.
- i.e., Raw Data ---> ML Algorithm Consumable data

### 1. Feature Transformation
- Datatype Conversion (from one form to another form).
- Generally, missing values handling, categorical features handling is performed.
- Also feature scaling and outlier detection is performed.
- e.g. In a cars dataset, kms_traveled feature is of type 'string', need to convert it to 'int' for model training.

### 2. Feature Construction
- Creating/Developing new feature using existing features
- Adding data which isn't directly available in data.
- e.g. We have a dataset in which height, weight is given calculating BMI on the basis of it.

### 3. Feature Selection
- Irrelevant features are present in dataset which aren't required during model development.
- Multiple similar features are present only relevant must be extracted.
- Performed using random forest, etc.

### 4. Feature Extraction
- Developing new features from existing but programmatically.
- Mainly used to reduce dimensionality of data by transforming it into new feature space.
- Algorithms like PCA, LDA are used to reduce dimensions of the data.
