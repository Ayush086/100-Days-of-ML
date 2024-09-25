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

## Problem Framing
**How to frame a problem statement in machine learning and how to build the solution for it ?**
- Let's say Netflix wants to increase their revenue and thought about 3 solutions:
      - new customer
      - extra charges
      - decrease frequency fo subscription cancellation (churn rate)
- I want to decrease the churn rate (got the problem)
- Now try to identify the type of the problem and it's end results of your solution whichever you thought about.
- Immediate solution will be decreasing the rate of subscription plans for already subscribed members.
- But that's not the perfect solution, we need to think more.
- It became a classification problem now. We need to determine what's customer's problem ? Why are they leaving the platform ?
- It may happen that subscription cancellation reason for every member isn't same.
- So try to identify the reason on the basis of sentiments. like
    - lack of content
    - high pricing
    - Bad UI
    - user counts per subscription
- Probability of willing to leave platform is different for every user (Now it became regression problem)
- Now, try to find out existing solution for your current problem (means solutions from other organizations)
- Data gathering, and understand it
- Also research for user data like,
  - browsing time
  - content left in middle
  - didn't find the searches
- the more you dig the more you will understand the problem and the more accurate will be the solution. 
