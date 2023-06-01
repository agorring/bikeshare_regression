# bikeshare_regression
A regression analysis to predict how many bikes will be rented from bike sharing company YouBike, based on a historical dataset.

Both XGBoost and random forest models displayed similar performances and are suitable for predicting the count of bike rentals. However, the recommended regression model for this application is XGBoost, which displayed the highest performance after remodelling (r-squared 0.899, RMSE 627). As well as boasting the highest performance, XGBoost is recommended over random forest for the following reasons:

• Better accuracy – the XGBoost algorithm does not construct trees to full depth. It counters overfitting by pruning trees at a certain point. The smaller trees allow the model to generalise better.

• Advanced hyperparameter tuning – the hyperparameters are set only for the first tree and adjust themselves iteratively. This makes the model more suited to input data which is real time and prone to variation. This may be beneficial for YouBike as the temperature, humidity, and windspeed are real time data inputs.

• XGBoost is designed to be memory efficient.
