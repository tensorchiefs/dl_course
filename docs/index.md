<head>
<style>
table, th, td {
    border: 0.5px solid black;
    vertical-align: top;
}
</style>
</head>

# Deep Learning (CAS machine intelligence) 

This course in deep learning focuses on practical aspects of deep learning. 

For the hands-on part we provide a docker container ([details and installation instruction](docker.md)).

## Other resources
We took inspiration (and sometimes slides / figures) from the following resources.

* Deep Learning Book (DL-Book) [http://www.deeplearningbook.org/](http://www.deeplearningbook.org/). This is a quite comprehensive book which goes far beyond the scope of this course.

* Convolutional Neural Networks for Visual Recognition [http://cs231n.stanford.edu/](http://cs231n.stanford.edu/), has additional material and [youtube videos of the lectures](https://www.youtube.com/playlist?list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC). While the focus is on computer vision, it also treats other topics such as optimization, backpropagation and RNNs. LKecture notes can be found at [http://cs231n.github.io/](http://cs231n.github.io/).

* More TensorFlow examples can be found at [dl_tutorial](https://github.com/oduerr/dl_tutorial/tree/master/tensorflow/) 

* Another applied course in DL: [TensorFlow and Deep Learning without a PhD](https://cloud.google.com/blog/big-data/2017/01/learn-tensorflow-and-deep-learning-without-a-phd)

## Syllabus (subject to change)
The course is split in 8 sessions, each 4 hours long. 


<table class="zebra" style="max-width:2200px;">
  <thead>
  <tr>
      <th style="text-align: left;" width="5">Day</th>
      <th style="text-align: left;" width="1700">Topic and slides</th>
      <th style="text-align: left;" width="120">Additional Material</th>
      <th style="text-align: left;" width="170">Exercises and homework</th></tr>
  </thead>

      <td style="text-align: left;" width="5">1</td>
      <td style="text-align: left;" width="170"> 
      		<b>Deep learning basics</b> <a href="https://www.dropbox.com/s/bvgd0wsp0zkgjm0/lecture01.pdf?dl=1">slides</a>
      		<ul>
      			<li>Overview of deep learning</li>
      			<li>Computational graphs, feeding and fetching</li>
      			<li>Loss function (crossentropy)</li>
      			<li>Gradient descent and generalizations</li>
      			<li>Example: linear regression</li>
      		</ul>
      </td>
      
      <td style="text-align: left;" width="120"> 
      	<ul>
        <li>
	Nature review article<a href='http://www.nature.com/nature/journal/v521/n7553/full/nature14539.html'>(LeCun, Bengio, Hinton, 2015)</a>
	</li>
	<li>
        DL-book chapter 6
	</li>
	<li>
	<a href="https://www.tensorflow.org/get_started/get_started">TensorFlow Intro</a>
	</li>
	
	</ul>
      </td>
      
      <td style="text-align: left;" width="170">
      	<ul>
		<li>
      			<a href='https://github.com/tensorchiefs/dl_course/tree/master/exercises/tf_matrix_mult.md'> Exercise MatrixMultiplication </a> 
      		</li>
			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/MatrixMultiplication_solution.ipynb'> Solution MatrixMultiplication </a> 
      		</li>
		<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/exercises/linreg_with_slider.md'> Exercise LinearRegression
 </a> 
      		</li>
			<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/Linreg_with_slider_solution.ipynb'> Solution LinearRegression </a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/simple_ops/Mandelbrot.ipynb'> Homework: Mandelbrot.ipynb</a> 
      		</li> 
      		<li>
      			<a href='https://github.com/tensorchiefs/dl_course/tree/master/exercises/Loading_Frozen_Graph.md'> Homework: Exercise Loading_Frozen_Graph (Artstyle Transfer)</a> 
      		</li>
      		<li>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/Loading_Frozen_Graph_solution.ipynb'> Homework: Solution Exercise Loading_Frozen_Graph (Artstyle Transfer)</a> 
      		</li>
			
         </ul>
      </td>
    </tr>
    
    <!---- Woche -->
    
    <tr>
      <td>2</td>
      <td> 
      		<b>Fully connected networks</b> <a href="https://www.dropbox.com/s/qmfh1ib3dzr50z5/lecture02.pdf?dl=1">slides</a>
      		<ul>
      			<li>Logistic regression</li>
      			<li>Multinomial Logistic Regression</li>
      			<li>Fully Connected networks</li>
      		</ul>
      </td>
      <td> 
      		DL-book chapter 6,7
      </td>
      <td>
      	<ul>
      		<li>
      			<a href='exercises_tf_playgound_day2.html'> TF-playground</a> 
      		</li>
      		
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/path_to_fc_nets/Multinomial%20Logistic%20Regression.ipynb'> Multinomial Logistic Regression.ipynb </a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/path_to_fc_nets/fcn_MNIST.ipynb'> fcn_MNIST.ipynb </a> 
      		</li>
      		</ul>
      </td>
    </tr>


    <!---- Woche -->

    <tr>
      <td>3</td>
      <td> 
      		<b>Tricks of the trade</b> <a href="XXX?dl=1">slides (TODO)</a>
      		<ul>
      			<li>Regularization:
      				<ul>
      					<li>Early stopping</li>
      					<li>L2 (Weight Decay)</li>
      					<li>Dropout</li>
      				</ul>
      			</li>
			<li>Backpropagation and Gradient Flow</li>
      		</ul>
      </td>
      <td> 
        <ul>
          <li>Backpropagation http://cs231n.github.io/optimization-2/</li>
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
      <td>4</td>
      <td> 
      		<b>Convolutional Neural Networks I</b> <a href="XXX?dl=1">slides (TODO)</a>
      		<ul>
      			<li>Introduction of CNNs:
      				<ul>
      					<li>What is convolution?</li>
      					<li>Feature/activation maps</li>
      					<li>How to train a CNN</li>
      				</ul>
      			</li>
			<li>CNN in action</li>
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
      					<li>Use pretrained nets for fine-tuning or feature generator</li>
      					<li>Understand CNN features</li>
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
      <td>6</td>
      <td> 
      		<b>Convolutional Neural Networks III</b> <a href="XXX?dl=1">slides (TODO)</a>
      		<ul>
   					<li>unsupervised learning, Autoencoder</li>
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
    
    
    
  </tbody>
</table>






