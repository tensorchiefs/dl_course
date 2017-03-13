## 8 faces with fully connected networks

In this excercise we work with the 8 faces dataset. this dataset has 350 images of 8 celebrities. To get an overview of the data open the notebook  
09_8_faces_overview and look at the celebrities and the images. The data is from a random sample of 8 persons  of the OXFORD VGG Face dataset (over 2600 Persons),  
for more information look here: http://www.robots.ox.ac.uk/~vgg/data/vgg_face/

a) Open the notebook 09_8_faces_only_fc and bulit this network and then train it.  
How good is the model? Look at the train valid and test accuracy.
```
____________________________________________________________________________________________________
Layer (type)                     Output Shape          Param #     Connected to                     
====================================================================================================
dense_1 (Dense)                  (None, 8)             55304       dense_input_1[0][0]              
____________________________________________________________________________________________________
activation_1 (Activation)        (None, 8)             0           dense_1[0][0]                    
====================================================================================================
Total params: 55,304
Trainable params: 55,304
Non-trainable params: 0
____________________________________________________________________________________________________
```
b) Now let's add some hidden layers to the network.  
Restart the notebook and built a new network with hidden layers, see below.  
How good is this model? Look at the train valid and test accuracy.
```
____________________________________________________________________________________________________
Layer (type)                     Output Shape          Param #     Connected to                     
====================================================================================================
dense_1 (Dense)                  (None, 400)           2765200     dense_input_1[0][0]              
____________________________________________________________________________________________________
activation_1 (Activation)        (None, 400)           0           dense_1[0][0]                    
____________________________________________________________________________________________________
dense_2 (Dense)                  (None, 200)           80200       activation_1[0][0]               
____________________________________________________________________________________________________
activation_2 (Activation)        (None, 200)           0           dense_2[0][0]                    
____________________________________________________________________________________________________
dense_3 (Dense)                  (None, 8)             1608        activation_2[0][0]               
____________________________________________________________________________________________________
activation_3 (Activation)        (None, 8)             0           dense_3[0][0]                    
====================================================================================================
Total params: 2,847,008
Trainable params: 2,847,008
Non-trainable params: 0
____________________________________________________________________________________________________
```
