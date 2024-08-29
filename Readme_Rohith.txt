Title: Sector-Wide Stock Market Prediction Using Time Series Analysis on Brazilian Equities

Purpose: the purpose of the code is to understand and analyse the patterns and trends of Brazilian Equities listed in the Brazil Stock Exchange using Time Series Analysis Techniques and methods and building the models which can predict the future course of stock values.

The methodology used is preprocessing of data for null values, and missing values, pivot dataset creation and data transformation like datetime transformation, and minmaxscaling.

VAR Model
Input: MinMaxScaled Dataset (scaled_df)
output: VAR Summary Regression Results Coefficients, standard error, t-stat value, and prob value of all the stocks listed in the data.
Forecasted Graphs

LSTM Model
create_lstm_model():
inputs: scaled dataset, look_back value
output: appended dataset for LSTM

LSTM Layers
4 Layers in total 2 LSTM Layers and 2 Dense Layers with Adam Optimizer and a Learning rate of 0.001 for the technique to prevent overfitting.


Using LSTM compiled model for predictions on X_test.

VAR Model - MAE: 0.021839769749166935, MSE: 0.0007210078107611017, RMSE: 0.026851588607773313, R2: -1.4862903543381507, MAPE: inf

LSTM Model - MAE: 0.06447768269184888, MSE: 0.01246257169253501, RMSE: 0.1116358889091452, R2: 0.6887253262456755, MAPE: inf

comparing the 2 models' evaluations it is evident that for predictions VAR model is better though the LSTM model is not too behind in terms of metrics which can also mean that both the models are efficient in the predictions and accuracy terms but when comparing the metrics of the values VAR is better than LSTM.

 