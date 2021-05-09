## Kaggle Project: Predict Future Sales
URL: https://www.kaggle.com/c/competitive-data-science-predict-future-sales
### Problem Statement

Reviewing daily historical sales records to make forecasts on the total monthly volume of products sold in **every** shop for **every** in the test set by experimenting with various models. 
This would allow store owners to have well-informed decisions on stock-taking at specific time of the year. 
Specifically, we are leveraging on qualities of **CNN-LSTM** model to help us generate such forecasts due to its comparatively lower MSE on both train and test set, which exhibits the best bias-variance tradeoff.

#### Data Dictionary
##### Important features to take note of:
|Feature|Type|Description|
|---|---|---|
|ID|*int*|ID that represents a (Shop,item) tuple within test set| 
|shop_id|*int*|unique identifier of a shop| 
|item_id |*int*|unique identifier of a product| 
|item_cnt_day |*float*|number of daily products sold|
|item_cnt_month |*float*|target variable: number of monthly products sold|
|date|*datetime*|date in format dd/mm/yyyy|


#### Conclusion/Recommendations
Based on the findings, we can draw several conclusions: <br>

1) The use of CNN-LSTM has an added advantage over parametric models due to its abilities to account for long term dependencies which are important in time series forecasts. 
> This is evident in the lower MSE in both train and validation set as compared to the linear models

2) On the public leaderboard, this model has earned a decent RMSE of 1.18651 