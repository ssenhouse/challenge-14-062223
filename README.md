# challenge-14-062223
 ---
 ## Machine Learning Trading
 ---
 ![fintech challenge14](/Starter_Code/images/14-4-challenge-image.png)
 
 ## Overview of Analysis
 The objective of this challenge is to create two algorithmic trading models using machine learning, analyze the results of the model and make a recommendation on which model is best. Additionally, I had to modify the training window and comment on the changes on the prediction 
 
 The baseline model used was a SVM (Support Vector Machine) learning model. The alternate model used was the DTC (DecisionTreeClassifier). 
 
## Results

# Model and Alternate Model baseline 

Figure 1 Baseline model
![baseline model](/Starter_Code/images/baseline.png)

The initial model has a 55% accuracy 

Figure 2 Alternate Model 1
![alternatemodel](/Starter_Code/images/alternatemodel.png)

The Alternate Model used a DecisionTreeClassifier model 

# Modified models increase the training data from 3 months to 6 months
Figure 3
![baseline_6month training](/Starter_Code/images/baseline_6month.png)

Figure 4
![alternate model 6month training](/Starter_Code/images/alternatemodel_6month.png)

# Modified models with 3 month training window but increase Short term moving average fast (SMA_Fast) to 10 days and long term moving average (SMA_Slow) to 90 days

Figure 5
![baseline 3month training 10 and 90days](/Starter_Code/images/baseline_3month_window_10_90days.png)

Baseline model using the training period to 3 months and the SMA_Fast = 10 day moving average, and SMA_Slow = 90 day moving average

