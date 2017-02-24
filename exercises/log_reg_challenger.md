## Logistic regression in TensorFlow

a) Open the notebook [log_reg_challenger](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/log_reg_challenger.ipynb) and run the fist 3 cells. 
We predict the the probability $p(y_i=1 | x_i)$ with the formula:
$$p(y_i=1 | x_i) = \frac{e^{(b + W' x_i)}}{1 + e^{(b + W' x_i)}} = \frac{1}{1 + e^{-(b + W' x_i)}}$$
Look at the predicted $p(y_i=1 | x_i)$ values with our given start parameters $W=-0.2$ and $b=20$. What do you observe? 

b) Now lets try to find better values for $W$ and $b$. Lets assume $W$ is given with $-1$. We want our probability $p(y_i=1 | x_i)$ to be $0.5$. What is the
value for $b$ in this case.  
Hint: at which $x$ value should $p(y_i=1 | x_i)$ be $0.5$, look at the data. $1 + e^{-(b + W' x_i)}$ must be $2$.

c) Run the TensorFlow forward pass in cell 5 and optimize the values for $W$ and $b$ in cell 6.  
Fetch the loss, W and b and print the final values.  
Hint: You can't use the same names for the results of your fetches as you have used for the TensorFlow graph. See cell 5.
 
