---
layout: default
mathjax: true
title: Deep Learning Course 
---
## Evaluate unsupervised learned MNIST features w.r.t. their suitability for classifying the corresponding digit labels

In the last excercise we have investigated the suitability of unsupervised learned features of MNIST data for pattern recognition in a 2D t-SNE plot.  Now we want to see if these features are useful to learn a classification for the digit label with only 100 labeled images as training data.
Open the notebook [17_MNIST_feature_evaluation](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/17_MNIST_feature_evaluation.ipynb).  
In this notebook we will train a fcNN classifier on the different versions of unsupervised learned MNIST features. We only use 100 trainig examples and then we use the trained fcNN to predict the label of 2000 digit images. A good feature representation should allow for efficient training with only few training data. Accordingly we compare the performace of the trained classifier to asses the suitability of the used features.

a) Built the network below in cell 9. Hint: Recall the shape of the input layer. Use a dropout probability of 0.4.

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

b) Which unsupervised learned feature respresentation is the best for the classification? Do you have an idea why?
