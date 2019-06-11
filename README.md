# ChatBot_V1
![](https://img.shields.io/badge/python-3.6.2-brightgreen.svg)  ![](https://img.shields.io/badge/tensorflow-2.0.0%2B-orange.svg)  ![](https://img.shields.io/badge/tensorlayer-2.0.2-yellowgreen.svg)


This project is intended to create an automatic reply system or ChatBot. It has been trained for twitter and cornell-movie dataset and currently supports both of them.
This project is the first version of more advance bot system project I am working upon.

## Motivation
The working of the automatic repy systems in online messengers and services fascinated me. In order to have more knowledge about their working, the basic need was to create a project to understand the basic needs of such a model and how to train it. The twitter and movie dataset is taken from their respective sources and are available under data. The coding style and motivation is found from <a href="https://github.com/tensorlayer/seq2seq-chatbot">seq-chatbot</a>. Tensorlayer is used as a high level wrapper over the tensorflow backend.

## Description
The project is created from Sequence to Sequence model and consists of two RNNs - an encoder and a decoder. The encoder reads the input sequence, word by word and emits a context, which would ideally capture the essence of the input sequence. Based on this context, the decoder generates the output sequence, one word at a time while looking at the context and the previous word during each timestep.
RNN are Recurrent Neural Networks in which nodes form a graph,hence they can be used to identify sequences in a text, as contrast with Feed Forward NN where there is no cycle.
![](http://complx.me/img/seq2seq/rnn.jpg)
 
 ## Working
 To run the application choose the required model. Modelv1t.npz is 1 epoch train model on twitter dataset. Modelv2t.npz is 15 epoch train model on twitter dataset and Modelcopper.npz is 15 epoch train model on cornel-movie dataset. Change the name in script accordingly.
 
1. To install the necessary requirements, follow the procedure
```python
pip install -r requirements.txt
```
2. Launch 'run.py' script to get query results provided in seeds.
 ```python
python run.py
```
3. To train the model on the required dataset launch 'main.py' script.
```python
python main.py
```
## Results
| **INPUT QUERY**        | **OUTPUT QUERY**      |
| ------------- |:-------------:| 
| How is the weather?     | i think it was a good one thing |
| How are you?      | i am so excited for the next time      |   
| I had an exam today. | thank you     |  
| Do you have any political views?   |  i am so excited for the debate  |
| Tell me something about yourself	 | i think its a lot of people     |  
|happy birthday have a nice day	  |  thank you  |

## Implementation
The 'main.py' script launches as:
<img src="https://github.com/AkhilDixit1998/ChatBot_V1/blob/master/ss/result3.png" height="450">
<br>
The time taken to run it is quite large.
<br>
<br>
The 'run.py' script launches as:
<img src="https://github.com/AkhilDixit1998/ChatBot_V1/blob/master/ss/result.png" height="450">
<img src="https://github.com/AkhilDixit1998/ChatBot_V1/blob/master/ss/result2.png" height="450">

#### Versions
1. Python- 3.6
2. Tensorflow- 2.0.0b0
3. Tensorlayer- 2.0.2

#### Code Working
The code working is provided in comments in the respective scripts.
