---
layout: default
mathjax: true
title: Deep Learning Course 
---
## MNIST_feature_evaluation

In the last excercise we compared different methods to extract features, now we want to see how we can use those features for a classification task.
Open the notebook [17_MNIST_feature_evaluation](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/17_MNIST_feature_evaluation.ipynb).  
In this notebook we will train a classifier on the extractet features of the MNIST dataset. We only use 100 trainig examples and predict 2000 digits. Eventually we compare the performace for all features extractiong methods, we used in excercise 16.

a) Built the network below in cell 9. Hint: remember the input layer. What is the inputshape? Use probability of 0.4.

```
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
dense_1 (Dense)              (None, 200)               6600      
_________________________________________________________________
batch_normalization_1 (Batch (None, 200)               800       
_________________________________________________________________
dropout_1 (Dropout)          (None, 200)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 10)                2010      
=================================================================
Total params: 9,410.0
Trainable params: 9,010.0
Non-trainable params: 400.0
_________________________________________________________________
``` 

b) Which features are the best for the classification and why?
