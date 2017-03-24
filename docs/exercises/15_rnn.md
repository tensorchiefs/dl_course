---
layout: default
mathjax: true
title: Deep Learning Course 
---
## Character Network


a)  **Before you open the notebook!**: Sometimes it's good to verify that keras really does what you want it to do. Therefore, calculate the number of parameters used for the first LSTM layer (line 4) and the dense layer (line 6 and 7). The notebook is defined as follows:

```
# maxlen = 40
# len(chars) = 106
model.add(LSTM(512, return_sequences=True, input_shape=(maxlen, len(chars))))  # original one
model.add(LSTM(512, return_sequences=True)) 
model.add(Dropout(0.2))
model.add(TimeDistributed(Dense(len(chars))))
model.add(TimeDistributed(Activation('softmax')))
```

Please note that a LSTM-layer has 4 units. Each unit takes the concatenation $[h_{t-1}, x_t]$ of the input vector $x_t$ and hidden state vector $h_{t-1}$ and transforms it using a matrix $W$ and a bias vector $b$. For example the forget-gate is [see also](http://colah.github.io/posts/2015-08-Understanding-LSTMs)

$$
 f_t = \sigma ([h_{t-1}, x_t] W_f + b_f)
$$  

**Solution:** (1'267'712) for first LSTM and (54'378) for dense layer. The solution can be found [here](15_rnn_solution_a.pdf)

b) Now open the notebook. Understand the code choose a different starting seed.

c) Play around with the temperature. What happens if you, increase / decrease the temperature.  
