# TV-Script-Generation
In this project, I generate my own Seinfeld TV scripts using RNNs using part of the Seinfeld dataset of scripts from 9 seasons. 
The Neural Network will generate a new ,"fake" TV script, based on patterns it recognizes in this training data.


### Model architecture :
  - Embedding layer to reduce the dimensionality of the input.
  - Two Long-Short-Term-Momort (LSTM) layers to detect patterns in trainging data.
  - One fully connected layer to predict the next word.
  
### Hyperparameters :
  - sequence_length = 8 
  - batch_size = 128
  - num_epochs = 10
  - learning_rate = 0.0005 with Adam optimizer.
  - input and output dim = number of unique words in dataset
  - embedding_dim = 300
  - hidden_dim = 512
  - added gradient clipping
  
### Dataset :
  - Seinfeld dataset [https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv]
    
 
  
