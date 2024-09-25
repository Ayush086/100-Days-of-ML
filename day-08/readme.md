# Today's Learnings
***Today I learned about the flow/process of model development in ML using real life example and provided dataset. Also learnt how to about the problem framing and how to choose the problem statement.***

## Placement Prediction (Toy Project)
- Let's assume we have a dataset containing 2 features(IQ, CGPA).
    - i.e., **|IQ  | CGPA|**
- Our task is to predict if the student is placed or not placed on the basis of IQ and CGPA.
- We are going to use Logistic Regression for the prediction.
    - Why Logistic Regression ?
        - LR is commonly used for classification/prediction
        - Best known to use for 2 categoriesd data
        - Draws decision boundary, which will differentiate between placed and unplaced student

### Project Flow
1. Import Dataset
2. Check Data
3. Data Preprocessing
4. Create some graph plots to check the behaviour of the data
5. Divide the input and result data
6. Scale values
7. Train Test Split
8. Train Models
9. Predict Values
10. Calculate Accuracy
11. Decision Boundary
12. Save Model (pickle)

**NOTE:** *Attached python notebook contains the implementation*
