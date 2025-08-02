# AN LSTM MODAL FOR PREDİCT THE TESLA STOCK PRİCE FROM 2010 TO 2020

I developed this mini project to better understand the LSTM algorithm in the context of time series prediction. The dataset includes the following variables: Date, Open, High, Low, Close, Adj Close, and Volume.

In this project, I use a sliding window approach where every 20 consecutive days are used to predict the 21st day's Close price, this window is referred to as a timestep.

To make accurate predictions, I utilized a powerful recurrent neural network architecture LSTM (Long Short-Term Memory), which is an improved version of traditional RNNs. I added an LSTM layer with 50 units and used the ReLU activation function. To prevent overfitting, I applied 20% dropout on this layer.

To further improve training efficiency and prevent overfitting, I also used early stopping and model saving techniques during training. This way, the training process automatically stops if the model stops improving, and only the best-performing version is kept. This helps avoid unnecessary training and ensures optimal results without overcomplicating the model.
