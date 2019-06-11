# ChatBot_V1
![](https://img.shields.io/badge/python-3.6.2-brightgreen.svg)
<br>
This project is intended to create an automatic reply system or ChatBot. It has been trained for twitter and cornell-movie dataset and currently supports both of them.
This project is the first version of more advance bot system project I am working upon.

## Motivation
The working of the automatic repy systems in online messengers and services fascinated me. In order to have more knowledge about their working, the basic need was to create a project to understand the basic needs of such a model and how to train it. The twitter and movie dataset is taken from their respective sources and are available under data. The coding style and motivation is found from <a href="https://github.com/tensorlayer/seq2seq-chatbot">seq-chatbot</a>.

## Description
The project is created from Sequence to Sequence model and consists of two RNNs - an encoder and a decoder. The encoder reads the input sequence, word by word and emits a context, which would ideally capture the essence of the input sequence. Based on this context, the decoder generates the output sequence, one word at a time while looking at the context and the previous word during each timestep.
RNN are Recurrent Neural Networks in which nodes form a graph,hence they can be used to identify sequences in a text, as contrast with Feed Forward NN where there is no cycle.
![](http://complx.me/img/seq2seq/rnn.jpg)
