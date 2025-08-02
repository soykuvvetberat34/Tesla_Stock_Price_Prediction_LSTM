# AN LSTM MODAL FOR PREDİCT THE TESLA STOCK PRİCE FROM 2010 TO 2020

I developed this mini project to better understand the LSTM algorithm in the context of time series prediction. The dataset includes the following variables: Date, Open, High, Low, Close, Adj Close, and Volume.

In this project, I use a sliding window approach where every 20 consecutive days are used to predict the 21st day's Close price, this window is referred to as a timestep.

To make accurate predictions, I utilized a powerful recurrent neural network architecture LSTM (Long Short-Term Memory), which is an improved version of traditional RNNs. I added an LSTM layer with 50 units and used the ReLU activation function. To prevent overfitting, I applied 20% dropout on this layer.

To further improve training efficiency and prevent overfitting, I also used early stopping and model saving techniques during training. This way, the training process automatically stops if the model stops improving, and only the best-performing version is kept. This helps avoid unnecessary training and ensures optimal results without overcomplicating the model.


--------------------------------



<img width="1011" height="531" alt="Başlıksız" src="https://github.com/user-attachments/assets/4e5d56da-019d-4b52-a4c2-b43af81591a2" />



This chart shows the historical closing prices of a stock from 2010 to 2020, highlighting a dramatic surge in value starting in late 2019


------------------------------



<img width="787" height="490" alt="image" src="https://github.com/user-attachments/assets/0adecd34-009d-497b-b353-000c6be057d6" />





This plot shows that both training and validation loss generally decrease over epochs, indicating improved model performance, though a slight fluctuation in validation loss suggests minor overfitting may have started.
