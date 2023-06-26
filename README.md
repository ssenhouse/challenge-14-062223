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
### **NOTE:** The training window for this model was 6 months 

Figure 5 Baseline model (SMA_Fast) = 10 (SMA_Slow) = 90 days
![baseline 3month training 10 and 90days](/Starter_Code/images/baseline_6month_window_10_90days.png)

Figure 6 Alternate model (SMA_Fast) = 10 (SMA_Slow) = 90 days
![alternate model 3month training 10 and 90days](/Starter_Code/images/alternatemodel_6month_window_10_90days.png)

# Evaluation Report (Summary & Analysis)
After comparing the results of the models after backtesting and classification, it is my recommendation that we use the SVM (Support Vector Machine) model, with a 6 month training span, and a 10 day fast and 90 slow simple moving averages (SMA). The predicted returns from this model trended better with the actual returns. The accuracy of the model was 56%, with a precision of predicting positive returns of 56% and a recall of 99%. 

Figure 7 Classification Table for Recommended model.
![classifcation report](/Starter_Code/images/classification_report.png)


## Baseline & Alternate Model Training Window = 3 months, SMA_Fast = 4 days, SMA_Slow = 100
* The inital baseline model (Figure 1) shows that the SVM model was prediciting values pre-2020 on trend with actual returns. Howver, after 2020 the model was predicting returns above trend of actual returns. 
* The alternate model was not useful in that it predicted the oppositive of the actual trends. 

## Baseline & Alternate Model Training Window = 6 months, SMA_Fast = 4 days, SMA_Slow = 100
* The baseline model was under trend prior to 2020, and over actual trend post 2020
* The alternate model shifted but still had instances where it trended the opposite of the actuals

## Baseline & Alternate Model Training Window = 3 months, SMA_Fast = 10 days, SMA_Slow = 90 days
* The baseline model predicted returns were trending above the actual returns prior to 2020. After 2020 trends for both the actual returns and predicted returns were similar.
* The alternate model predicted returns did not trend well with the actual returns and therefore was not a good model.  
