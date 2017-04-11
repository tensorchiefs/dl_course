---
layout: default
mathjax: true
title: Deep Learning Course 
---
## 8 faces fine tuning
 
In this excercise we work with the 8 faces dataset. We want to improve the performance by using a  
pretrained vgg16 network. We predict the features on the fc1 layer with the already learned weights on imagenet 
and then train a small fully connected network for our own labels. The feature extraction was done in this notebook 
[vgg16_feature_extraction_8_faces](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/12_vgg_feature_extraction_without_relu_8_faces.ipynb)

a) What do you expect, will it increase our performance? Why? What's the idea behind this so called fine tuning?


b) Open the notebook [8 faces fine tuning](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/12_8_faces_fine_tuning.ipynb) and bulit this network and then train it.  
```
____________________________________________________________________________________________________
Layer (type)                     Output Shape          Param #     Connected to                     
====================================================================================================
dense_1 (Dense)                  (None, 400)           1638800     dense_input_1[0][0]              
____________________________________________________________________________________________________
batchnormalization_1 (BatchNorma (None, 400)           1600        dense_1[0][0]                    
____________________________________________________________________________________________________
activation_1 (Activation)        (None, 400)           0           batchnormalization_1[0][0]       
____________________________________________________________________________________________________
dropout_1 (Dropout)              (None, 400)           0           activation_1[0][0]               
____________________________________________________________________________________________________
dense_2 (Dense)                  (None, 400)           160400      dropout_1[0][0]                  
____________________________________________________________________________________________________
batchnormalization_2 (BatchNorma (None, 400)           1600        dense_2[0][0]                    
____________________________________________________________________________________________________
activation_2 (Activation)        (None, 400)           0           batchnormalization_2[0][0]       
____________________________________________________________________________________________________
dropout_2 (Dropout)              (None, 400)           0           activation_2[0][0]               
____________________________________________________________________________________________________
dense_3 (Dense)                  (None, 8)             3208        dropout_2[0][0]                  
____________________________________________________________________________________________________
activation_3 (Activation)        (None, 8)             0           dense_3[0][0]                    
====================================================================================================
Total params: 1,805,608
Trainable params: 1,804,008
Non-trainable params: 1,600
____________________________________________________________________________________________________
```

b) Complete the code to get the predicted labels out of the probability vector and look at the accuracy on the  
test data.  
