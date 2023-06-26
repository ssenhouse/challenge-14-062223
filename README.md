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

Figure 2 Alternate Model 1
![alternatemodel](/Starter_Code/images/alternatemodel.png)

# Modified models increase the training data from 3 months to 6 months

Figure 3 Baseline Model with 6 month training window
![baseline_6month training](/Starter_Code/images/baseline_6month.png)

Figure 4 Alternate model with 6 month training window
![alternate model 6month training](/Starter_Code/images/alternatemodel_6month.png)

# Modified models SMA_Fast and SMA_Slow to 10 and 90 days respectively

Figure 5 Baseline model (SMA_Fast) = 10 (SMA_Slow) = 90 days
![baseline 3month training 10 and 90days](/Starter_Code/images/baseline_3month_window_10_90days.png)


Figure 6 Alternate model (SMA_Fast) = 10 (SMA_Slow) = 90 days
![alternate model 3month training 10 and 90days](/Starter_Code/images/alternatemodel_3month_window_10_90days.png)