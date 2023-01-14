# Stock Market Predections.

Time Series data is a series of data points indexed in time oreded fation.
So it makes a challange to predicet Timeseries data, In this project we will analyize and predict some stocks from tech-companies (Apple, Microsoft, Dell , Google).

This project is spereated in 3 jupyter notebook files.
* EDA 
* Feature Enginering and XGBoost
* LSTM_Timeseries
  

## 1- EDA

In this jupyter notebook we download the data using `yfinance`
It is one of the most famous models in python which is used to collect finance data online using the yahoo engine.

Then we explore the data and see how the data set is formed and how we are going to adjust it, then we make some analysis on the data using `matplotlib` and `seaborn`.

So we can see that there is a trending increase in the closing price of the stocks and it is seasonal increase.


## 2- Feature Enginering and XGBoost

In this jupyter notebook we adjust the the data to improve the models preformance, as we explored in the `EDA.ipynb` there is a seasonal increase in the stocks, from that we can add some featuers or columns in the data useing the `Date` column (index).

Then we start training or models in the notebook I chose `XGBRegressor`, I set the models params and I trained and tested the model on the data we split before,
The `XGBRegressor` was not a good choice for this case then we move to the next notebook.

## 3- LSTM_Timeseries

In the previous notebook we learned that `XGBRegressor` was not a good fit for Time series data because beside the Linear increase in the stock prices there is a seasonal increase that the previous model can not predict so we move to the next model `LSTM`.

LSTM : Long Short-Term Memory, It is a RNN model used for this usecase ( Timeseries Predictions).