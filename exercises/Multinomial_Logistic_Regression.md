## Multinomial Logistic Regression on MNIST dataset

a) Open the notebook [Multinomial Logistic Regression](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/Multinomial_Logistic_Regression.ipynb).
In this notebook we use multinomial logistic regression to predict the handwritten digits of the MNIST dataset.  
We have 4000 examples with 784 pixel values and 10 classes. Run the fist 3 cells and explain the one-hot-encoding. In TensorFlow we need to use one-hot-encoding. 

b) Write the missing TensorFlow code in cell 4 to do the required matrix multiplication between x and w and then add the bias b.  
$z=x*w+b$

c) Run the next two cells to store the graph and do a forward pass of the untrained network, look at the probability for each class of some examples.

c) Now lets train the model. We use a mini-batch size of 128 and use the fist 2400 examples for training.  
The validation set will be the examples from 2400 to 3000. Write the code to get the loss and the probabilities of your validation set.
Run the last cells to check the performance of the model and to get the probability of a random example of the validation set.