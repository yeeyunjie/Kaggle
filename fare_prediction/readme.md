## Kaggle Project: Predict New York's Taxi Fares
URL: https://www.kaggle.com/c/new-york-city-taxi-fare-predictions

### Problem Statement

Always wondered about the costs of transportation when planning your budget? This model aims to provide accurate estimations of transport expenditure when taking taxis in New York. In addition, it might provide a good gauge as to how much a taxi fare should be so as to not be fooled!
Specifically, we are leveraging on qualities of **ANN** model to help us predict the `fare_amount` due to its comparatively lower MSE on both train and test set, which exhibits the best bias-variance tradeoff.

#### Data Dictionary
##### Important features to take note of:
|Feature|Type|Description|
|---|---|---|
|key|*string*|Unique ID that represents each row in train/test set| 
|pickup_datetime|*datetime*|timestamp value indicating when the taxi ride started| 
|pickup_longitude|*float*|longitude coordinate of where the taxi ride started.| 
|pickup_latitude|*float*|latitude coordinate of where the taxi ride started.|
|dropoff_longitude|*float*|longitude coordinate of where the taxi ride ended.|
|dropoff_latitude*float*|latitude coordinate of where the taxi ride ended.|
|passenger_count |*int*|number of passengers in the taxi ride|
|fare_amount|*float*|Cost of taxi ride - target variable|

#### Conclusion/Recommendations
Based on the findings, we can draw several conclusions: <br>

1) Neural Nets is better able to learn the relationship between the predictor variables and the cab fare. 
> This is evident in the lower MAE in both train and validation set as compared to the linear models

2) On the public leaderboard, this model has earned a decent RMSE of 3.866 