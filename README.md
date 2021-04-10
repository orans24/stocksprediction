# stocksprediction
on the code you got the option to :
1. build data set to train the model

2. train the model

3.check model preformence

4.predict the the stocks movment.

to activate the code all you need to do is to insert the ticker of the stocks you would like to predict.
you can see as example the data set, model and  predction for 04/08/21 that create for apple,google,microsoft and facebook.
notes:
the code predict the next 10 days depanding on 25 last days,to train the model i use the historical data of the stocks since the day it tag to NASDAQ against the movment of 
russel,nasdaq,djowns and s&p.
model architecture:
input layer : lstm 512 units defualt activations and 0.2 dropout.
hidden layers: 2 lstm layers defualt activiations first one with 256 units and second with 128 both 0.2 dropout.
output layer: dense layer with 10 units and activation sigmoid.
compile with loss:mse,optimizer:adam,metrics:mae.
batch size for fit 32 and 300 epoch 
