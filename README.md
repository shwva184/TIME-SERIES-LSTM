# TIME-SERIES-LSTM

Using LSTM to predict the adjusted closing price to get a better idea of the overall value of the stock. Data used is from https://finance.yahoo.com/quote/%5EGSPC/history

I have taken a snippet of the data from 1990 to 2018.
There are 4 features.
Prediction is done for adjusted closing price.

The time series has been split into shorter series of 30 data points , approximately time series of a month.

90% of the data is used for training and 10% for validation.

Applied model summary is as follows :

![alt text](https://github.com/shwva184/TIME-SERIES-LSTM/blob/main/Capture1.PNG?raw=true)

Predicted output : 

![alt text](https://github.com/shwva184/TIME-SERIES-LSTM/blob/main/Capture.PNG?raw=true)



Inspired by : https://github.com/BenjiKCF/Neural-Net-with-Financial-Time-Series-Data
