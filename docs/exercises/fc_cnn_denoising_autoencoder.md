---
layout: default
mathjax: true
title: Deep Learning Course 
---
## Fully connected and convolutional autoencoder on MNIST

Open the notebook [16_fc_cnn_denoising_autoencoder_solution](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/16_fc_cnn_denoising_autoencoder_solution.ipynb) and run all cells.  
Try to understand the code.

a) Look at first fully connected autoencoder. Why is there a sigmoid-activation in the last layer? What is the size of the bottleneck layer?  Hint: What is the range of the input data and want is the goal of the autoencoder.
```
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
bottleneck (Dense)           (None, 32)                25120     
_________________________________________________________________
reconstruction (Dense)       (None, 784)               25872     
=================================================================
Total params: 50,992.0
Trainable params: 50,992
Non-trainable params: 0.0
_________________________________________________________________
``` 

b) What is the difference between the fc autoencoder and the denoising fc autoencoder?

c) Why are there much less weights in the cnn autoencoders.

d) Compare the the five tsne-plots. What do you think, which one is the best?