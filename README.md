# TIME-SERIES-LSTM

Using LSTM to predict the adjusted closing price to get a better idea of the overall value of the stock. Data used is from https://finance.yahoo.com/quote/%5EGSPC/history

I have taken a snippet of the data from 1990 to 2018.
There are 4 features.
Prediction is done for adjusted closing price.

The time series has been split into shorter series of 30 data points , approximately time series of a month.

90% of the data is used for training and 10% for validation.

Applied model summary is as follows :

_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 lstm_12 (LSTM)              (None, 30, 128)           68096     
                                                                 
 dropout_12 (Dropout)        (None, 30, 128)           0         
                                                                 
 lstm_13 (LSTM)              (None, 128)               131584    
                                                                 
 dropout_13 (Dropout)        (None, 128)               0         
                                                                 
 dense_12 (Dense)            (None, 64)                8256      
                                                                 
 dense_13 (Dense)            (None, 1)                 65        
                                                                 
=================================================================

Total params: 208,001
Trainable params: 208,001
Non-trainable params: 0
________________________

Predicted output : 
![alt text](http://github.com/shwva184/TIME-SERIES-LSTM/edit/main/Capture.png)



Inspired by : https://github.com/BenjiKCF/Neural-Net-with-Financial-Time-Series-Data
