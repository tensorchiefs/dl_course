## Logistic regression in TensorFlow

a) Open the notebook [log_reg_challenger](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/04_log_reg_challenger.ipynb). In this notebook
we use (binary) logistic regression to predict the probability for an O-ring to show a damage
$(y=1)$ by using the temperature during take-off as predictor $x$.  
$$p(y_i=1 | x_i) = \frac{e^{(b + W' x_i)}}{1 + e^{(b + W' x_i)}} = \frac{1}{1 + e^{-(b + W' x_i)}}$$
Determine the predicted $p(y_i=1 | x_i)$ values when using the parameters $W=-0.2$ and $b=20$. What do you observe?

b) Now lets try to find better values for $W$ and $b$. Lets assume $W$ is given with $-1$. We want the probability
for a damage $p(y_i=1 | x_i)$ to be $0.5$.  
Determine an appropriate value for $b$.  
Hint: at which $x$ value should $p(y_i=1 | x_i)$ be $0.5$, look at the data. At this $x$ value the term $1 + e^{-(b + W' x_i)}$ must be $2$.

c) Now we want to optimize the parameter values by using the gradient descent
method. Run the TensorFlow forward pass in cell 5 and optimize the values for $W$ and $b$ in cell 6.  
Fetch the loss, $W$ and $b$ and print the final values.  
Hint: You can't use the same names for the results of your fetches as you have used for the TensorFlow graph. See cell 5.
 
