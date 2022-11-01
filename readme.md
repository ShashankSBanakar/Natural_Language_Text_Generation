Language Modeling 

A Langauge Model is simply a probability distribution over words conditioned on the words that have appeared in the 
sentence / text so far.

The recurrent neural network model used to achieve this task is an LSTM - Long Short Term Memory.

![model](https://user-images.githubusercontent.com/103943776/199201471-bf88f661-61b3-4aed-b24e-819c83f804b8.png)

LSTMs can not only remember the context of the text based on current time stamp but also can remember longer 
contexts. The hidden state in an LSTM has two parts: a hidden state which remembers the short term context while
the cell state is responsible to remember the influences of a much longer term. When both, the short term and long
term contexts, can be taken care of, it's possible for the model to predict the next word after passing a word or 
sequence of words to the model. When done iteratively, the model will be able to generate text by itself after
the model is given a sequence of words to start from.

![Screenshot (12)](https://user-images.githubusercontent.com/103943776/199201601-bde66e40-ccc6-4305-859c-52702d3d6cef.png)

Since the model has not been trained on a large enough corpus and for not enough number of epochs due to limited GPU resources available, the the text generated by the model doesn't make much sense but the model is able to generate text as expected nonetheless.

Language Modeling has several fascinating applications including text summerization, machine translation systems, question answering and speech recognition.

The text used to train the LSTM model in this project is a dataset from kaggle: https://www.kaggle.com/datasets/nbroad/feedback-prize-linebyline-text-dataset

