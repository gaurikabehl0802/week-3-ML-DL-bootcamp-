## Project Overview
The Metro Interstate Traffic Volume Prediction project is designed to forecast hourly traffic flows on the I-94 interstate highway. 
Traffic density fluctuates heavily based on the time of day, day of the week, holidays, and weather variations like rain, snow, or cloud coverage. 
By applying machine learning, the project captures these intricate, non-linear relationships to accurately predict vehicle volume, providing data-driven insights that can assist in urban traffic management and congestion planning
## Summary of Benchmark Results
To find the best predictive model, three distinct ensemble architectures were evaluated on the dataset:
1. XGBoost (Gradient Boosting) delivered the best performance, achieving the highest $R^2$ score and lowest error (RMSE). Its sequential tree-building optimization excels at correcting past errors step-by-step, making it highly effective at handling complex hourly peak traffic surges.
2. Random Forest (Bagging) performed strongly and came in a close second place. Building multiple independent deep trees in parallel provides excellent stability and makes it incredibly robust against noisy fluctuations in weather data.
3. AdaBoost scored the lowest overall. It typically relies on shallow decision trees (or "stumps") that struggle to map the deep, intersecting temporal relationships—like the combination of rush hours with specific weekdays—required for accurate traffic forecasting.
