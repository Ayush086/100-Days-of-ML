# Today's Learnings
 **How ML models run on servers ?**

 ## Batch/Offline ML
 - *In this type of learning model is trained on static data (dataset) and performs operations based on the training data.*
 - Whole data is feed at one time for the training, before deployment all the training process is performed and then it's deployed on servers.
 - Also called as static model.
 - eg. Image Classification, etc.

  *Periodic training is performed to improve the performance of static ML model.*
  
  ### Periodic Training
  - Re-training static model after some span of time.
  - It's not a continuous process.
  - Interval isn't fixed.


## Online ML
- *model training operates on real-time data.*
- Initially some data is provided to model for basic training purpose, but after deployment it keeps improving it's performance as new data is feeded.
- eg. stock market analysis.

  *Learning Rate is predefined for smooth processing.*
  
  ### Learning Rate
  - Setting a fixed time interval for model to collect real time data and train itself with that data.
  - If learning rate is not fixed correctly then model may out perform
  - *In frequent training model can't keep track of old data and it may lead to model failure*
