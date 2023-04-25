# Text_prediction
The model will consider the last word of a particular sentence and predict the next possible word. We will be using methods of natural language processing, language modeling, and deep learning. We will start by analyzing the data followed by the pre-processing of the data. We will then tokenize this data and finally build the deep learning model. The deep learning model will be built using LSTM’s

Pre-processing the Dataset:
The first step is to remove all the unnecessary data from the Metamorphosis dataset. We will delete the starting and end of the dataset.

Tokenization: Tokenization refers to splitting bigger text data, essays, or corpus’s into smaller segments. These smaller segments can be in the form of smaller documents or lines of text data. 

Creating the Model:
We will be building a sequential model. We will then create an embedding layer and specify the input dimensions and output dimensions. It is important to specify the input length as 1 since the prediction will be made on exactly one word and we will receive a response for that particular word.
We will then add an LSTM layer to our architecture.
The softmax activation ensures that we receive a bunch of probabilities for the outputs equal to the vocab size.

Prediction:
For the prediction notebook, we will load the tokenizer file which we have stored in the pickle format. We will then load our next word model which we have saved in our directory.

Observation:
We are able to develop a high-quality next word prediction for the metamorphosis dataset. We are able to reduce the loss significantly in about 115 epochs. The next word prediction model which we have developed is fairly accurate on the provided dataset. The overall quality of the prediction is good.
