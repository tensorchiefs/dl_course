
# Deep Learning (CAS machine intelligence) 

This course in deep learning focuses on practical aspects of deep learning. 

For the hands-on part we provide a docker container ([details and installation instruction](docker.md)).

## Other resources
We took inspiration (and sometimes slides / figures) from the following resources.

* Deep Learning Book (DL-Book) [http://www.deeplearningbook.org/](http://www.deeplearningbook.org/). This is a quite comprehensive book which goes far beyond the scope of this course.

* Convolutional Neural Networks for Visual Recognition [http://cs231n.stanford.edu/](http://cs231n.stanford.edu/), has additional material and [youtube videos of the lectures](https://www.youtube.com/playlist?list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC). While the focus is on computer vision, it also treats other topics such as optimization, backpropagation and RNNs. Lecture notes can be found at [http://cs231n.github.io/](http://cs231n.github.io/).

* More TensorFlow examples can be found at [dl_tutorial](https://github.com/oduerr/dl_tutorial/tree/master/tensorflow/) 

* Another applied course in DL: [TensorFlow and Deep Learning without a PhD](https://cloud.google.com/blog/big-data/2017/01/learn-tensorflow-and-deep-learning-without-a-phd)

## Syllabus (subject to change)
The course is split in 8 sessions, each 4 hours long. 


<table class="zebra" style="max-width:900px;">
  <tr>
      <th style="text-align: left;" width="5">Day</th>
      <th style="text-align: left;" width="350">Topic and slides</th>
      <th style="text-align: left;" width="200">Additional Material</th>
      <th style="text-align: left;" width="200">Exercises and homework</th></tr>


      <td style="text-align: left;" width="5">1</td>
      <td style="text-align: left;" width="350"> 
      		<b>Deep learning basics</b> <a href="https://www.dropbox.com/s/bvgd0wsp0zkgjm0/lecture01.pdf?dl=1">slides</a>
      		<ul>
      			<li>Overview of deep learning</li>
      			<li>Computational graphs, feeding and fetching</li>
      			<li>Loss function (crossentropy)</li>
      			<li>Gradient descent and generalizations</li>
      			<li>Example: linear regression</li>
      		</ul>
      </td>
      
      <td style="text-align: left;" width="200"> 
      	<ul>
        <li>
	<a href='http://www.nature.com/nature/journal/v521/n7553/full/nature14539.html'>Nature review article</a>
	</li>
	<li>
        DL-book chapter 6
	</li>
	<li>
	<a href="https://www.tensorflow.org/get_started/get_started">TensorFlow Intro</a>
	</li>
	
	</ul>
      </td>
      
      <td style="text-align: left;" width="200">
      	<ul>
		<li>
      			<a href='http://htmlpreview.github.io/?https://github.com/tensorchiefs/dl_course/blob/master/exercises/day1.html'> Exercises day1 </a> 
      		</li>
			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/01_MatrixMultiplication_solution.ipynb'> Solution MatrixMultiplication </a> 
      		</li>

			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/02_Linreg_with_slider_solution.ipynb'> Solution LinearRegression </a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/simple_ops/Mandelbrot.ipynb'> Homework: Mandelbrot.ipynb</a> 
      		</li> 
 
      		<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/03_Loading_Frozen_Graph_solution.ipynb'> Homework: Solution Exercise Loading_Frozen_Graph (Artstyle Transfer)</a> 
      		</li>
			
         </ul>
      </td>

    
    <!---- Woche -->
    
    <tr>
      <td>2</td>
      <td> 
      		<b>Multinomial Logistic Regression</b> <a href="https://www.dropbox.com/s/qmfh1ib3dzr50z5/lecture02.pdf?dl=1">slides</a>
      		<ul>
      			<li>Logistic regression</li>
      			<li>Multinomial Logistic Regression</li>
      		</ul>
      </td>
      <td> 
      		DL-book chapter 6
      </td>
      <td>
      	<ul>
      		<li>
      			<a href='exercises_tf_playgound_day2.html'> TF-playground</a> 
      		</li>
		<li>		
      			<a href='http://htmlpreview.github.io/?https://github.com/tensorchiefs/dl_course/blob/master/exercises/day2.html'> Exercises day2  </a> 
      		</li>
			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/04_log_reg_challenger_solution.ipynb'> Solution Logistic Regression </a> 
      		</li>
      		
			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/05_Multinomial_Logistic_Regression_solution.ipynb'> Solution Multinomial Logistic Regression </a> 
      		</li>
		


      		</ul>
      </td>
    </tr>


    <!---- Woche -->

    <tr>
      <td>3</td>
      <td> 
		<b>Going Deeper / Tricks of the trade</b> <a href="https://www.dropbox.com/s/vkud41xsb7pz3tz/lecture03.pdf?dl=1">slides </a>
      		<ul>
			<li>Fully connected network</li>
			<li>Backpropagation and Gradient Flow</li>
			<li>ReLU</li>
			<li>Regularization:
      				<ul>
      					<li>Early stopping</li>
      					<li>L2 (Weight Decay)</li>
      					<li>Dropout</li>
      				</ul>
      			</li>
			
      		</ul>
      </td>
      <td> 
        <ul>
          <li> <a href='http://cs231n.github.io/optimization-2/'> Backpropagation </a>  </li>
	  <li> DL-book chapter 7 (for regularization)</li>
        </ul>
      </td>
      <td>
      	<ul>
	<li>
	      			<a href='http://htmlpreview.github.io/?https://github.com/tensorchiefs/dl_course/blob/master/exercises/day3.html'> Exercises day3 </a> 
      		</li>
			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/06_fcn_MNIST_solution.ipynb'> Solution Fully Connected Network MNIST  </a> </li>
			<li>
			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/07_fcn_MNIST_keras_solution.ipynb'> Solution Fully Connected network (Tricks of the Trade)</a> 
      			</li>

         </ul>
      </td>
    </tr>
       
    <!---- Woche -->
    <tr>
      <td>4</td>
      <td> 
      		<b>Convolutional Neural Networks I</b> 
		<a href="https://www.dropbox.com/s/4pc1z5b55uuvwi0/CNN-Tag4-CNN-plan-v1.pdf?dl=1">slides</a>
      		<ul>
		        <li>Batch-Normalization</li>
      			<li>Why going beyond fully connected NN?</li> 
      			<li>What is convolution?</li>      			
      			<li>Building a CNN</li>
			<li>Simlarities between a CNN and the brain</li>
      		</ul>
      </td>
      <td> 
        <ul>
		<li>
	<a href="https://github.com/vdumoulin/conv_arithmetic">Convolution arithmetic</a>
	</li>
        </ul>
      </td>
      <td>
      	<ul>
      		<li>
      			TODO
      		</li>
      		<li>
      			 TODO
      		</li> 
      		<li>
      			TODO
      		</li>
         </ul>
      </td>
    </tr>
    <!---- Woche -->
    <tr>
      <td>5</td>
      <td> 
      		<b>Convolutional Neural Networks II</b> <a href="XXX?dl=1">slides (TODO)</a>
      		<ul>
   					<li>Typical CNN architectures</li>
					<li>Feature/activation maps in detail</li>
					<li>Understand CNN features</li>
      					<li>Use pretrained nets for fine-tuning or feature generator</li>
      					
      		</ul>
      </td>
      <td> 
        <ul>
		<li>
	TODO
	</li>
	<li>
	<a href="http://yosinski.com/deepvis">Understanding CNNs through visualization</a>
	</li>
	<li>
	<a href="http://cs.stanford.edu/people/karpathy/convnetjs/demo/cifar10.html">demo CNN and activation maps</a>
	</li>
	<li>
	<a href="https://blog.keras.io/category/demo.html">Use keras to visualize which image features activate a feature map</a>
	</li>

        </ul>
      </td>
      <td>
      	<ul>
      		<li>
      			TODO
      		</li>
      		<li>
      			 TODO
      		</li> 
      		<li>
      			TODO
      		</li>
         </ul>
      </td>
    </tr>
    <!---- Woche -->
    <tr>
      <td>6</td>
      <td> 
      		<b>Un- and Semi-supervised Learning</b> <a href="XXX?dl=1">slides (TODO)</a>
      		<ul>
   					<li>Autoencoder</li>
					<li>denoising Autoencoder</li>
      					<li>semi-supervised learning</li>
      					<li>TODO</li>
      		</ul>
      </td>
      <td> 
        <ul>
		<li>
	TODO
	</li>

        </ul>
      </td>
      <td>
      	<ul>
      		<li>
      			TODO
      		</li>
      		<li>
      			 TODO
      		</li> 
      		<li>
      			TODO
      		</li>
         </ul>
      </td>
    </tr>

    
    <!---- Woche -->
     <tr>
      <td>7</td>
      <td> 
      		<b>Recurent Neural Networks</b> <a href="XXX?dl=1">slides</a>
      		<ul>
      			<li>Recurrent Neural Networks</li>
      			<li>Vanishing Gradient Problem</li>
      			<li>LSTMs</li>
      		</ul>
      </td>
      <td> 
        <ul>
          <li>Karpathy (May 2015) The unreasonable effectiveness of Recurrent Neural Networks <a href='http://karpathy.github.io/2015/05/21/rnn-effectiveness/'>(blog post)</a></li>
	  
          <li>Colah (August 2015) Understanding LSTM Networks <a href='http://colah.github.io/posts/2015-08-Understanding-LSTMs/
          '>(blog post)</a></li>
        </ul>
      </td>
      <td>
      	<ul>
      		<li>
      			TODO
      		</li>
      		<li>
      			 TODO
      		</li> 
      		<li>
      			TODO
      		</li>
         </ul>
      </td>
    </tr>
    
    
    
 
</table>






