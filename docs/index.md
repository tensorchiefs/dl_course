---
layout: default
title: Deep Learning Course 
---
# Deep Learning (CAS machine intelligence) 

This course in deep learning focuses on practical aspects of deep learning. 

For the hands-on part we provide a docker container ([details and installation instruction](docker.md)).

## Other resources
We took inspiration (and sometimes slides / figures) from the following resources.

* Deep Learning Book (DL-Book) [http://www.deeplearningbook.org/](http://www.deeplearningbook.org/). This is a quite comprehensive book which goes far beyond the scope of this course.

* Convolutional Neural Networks for Visual Recognition [http://cs231n.stanford.edu/](http://cs231n.stanford.edu/), has additional material and [youtube videos of the lectures](https://www.youtube.com/playlist?list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC). While the focus is on computer vision, it also treats other topics such as optimization, backpropagation and RNNs. Lecture notes can be found at [http://cs231n.github.io/](http://cs231n.github.io/).

* More TensorFlow examples can be found at [dl_tutorial](https://github.com/oduerr/dl_tutorial/tree/master/tensorflow/) 

* Another applied course in DL: [TensorFlow and Deep Learning without a PhD](https://cloud.google.com/blog/big-data/2017/01/learn-tensorflow-and-deep-learning-without-a-phd)

## Syllabus
The course is split in 8 sessions, each 4 hours long. 

<table class="zebra" style="max-width:900px">

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
      		01 Matrix Multiplication 
          <a href="exercises/01_tf_matrix_mult"> Exercises</a> | 
          <a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/01_MatrixMultiplication.ipynb'> Notebook</a> | 
          <a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/01_MatrixMultiplication_solution.ipynb'> Solution</a> 
      		</li>

			<li>
      		02 Linreg (with_slider_solution) 
          <a href="exercises/02_linreg_with_slider"> Exercises</a> |
          <a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/02_Linreg_with_slider.ipynb'> Notebook</a> 
          <a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/02_Linreg_with_slider_solution.ipynb'> Solution LinearRegression </a> 
      </li>

      <li>
            03 Homework: Frozen Graph (Artstyle Transfer)
            <a href="exercises/03_Loading_Frozen_Graph"> Exercises</a> |
            <a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/03_Loading_Frozen_Graph_solution.ipynb'> Solution Exercise</a> 
      </li>

      		<li>
      			 Homework: Mandelbrot <a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/simple_ops/Mandelbrot.ipynb'> Notebook</a> 
      		</li> 
 
      		
			
         </ul>
      </td>

    
    <!-- Woche -->
    
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
            04 Logistic Regression (Challenger)<a href="exercises/04_log_reg_challenger"> Exercises</a> | 
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/04_log_reg_challenger_solution.ipynb'> Solution </a> 
      		</li>
      		
			<li>
            05 Multinomial Logistic Regression  <a href="exercises/05_Multinomial_Logistic_Regression"> Exercises</a>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/05_Multinomial_Logistic_Regression_solution.ipynb'> Solution</a> 
      </li>
		


      		</ul>
      </td>
    </tr>


    <!-- Woche -->

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
            06 Fully Connected Network MNIST <a href="exercises/06_fcn_MNIST"> Exercises</a>
      			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/06_fcn_MNIST_solution.ipynb'> Solution  </a> 
      </li>
      			<li> 07 Fully Connected network (Tricks of the Trade)
			<a href="exercises/07_fcn_MNIST_tricks"> Exercises</a>
			<a href='https://github.com/tensorchiefs/dl_course/blob/master/notebooks/07_fcn_MNIST_keras_solution.ipynb'> Solution </a> 
      			</li>

         </ul>
      </td>
    </tr>
       
    <!-- Woche -->
    <tr>
      <td>4</td>
      <td> 
      		<b>Convolutional Neural Networks I</b> 
		<a href="https://www.dropbox.com/s/99qgtofbao5je8t/CNN-Tag4-CNN-presented.pdf?dl=1">slides</a>
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
	<li>
	<a href="http://cs.stanford.edu/people/karpathy/convnetjs/demo/cifar10.html">demo CNN and activation maps</a>
	</li>
        </ul>
      </td>
      <td>
      	<ul>
	
	      		<li> finger-exercise ReLu
			<a href="https://www.dropbox.com/s/yogcjidr7ng3qtb/08a-Schnelluebung-ReLu.pdf?dl=1"> Exercise</a>|
			<a href='https://www.dropbox.com/s/d1se84xdui3uwqz/08a-Schnelluebung-ReLu-solution.pdf?dl=1'> Solution </a> 
	
      		</li>
<li>

			08 CNN <a href="exercises/08_CNN_MNIST"> Exercises</a>
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/08_cnn1_mnist.ipynb">Solution CNN1 with centered MNIST</a>|
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/08_cnn1_mnist_no_centering.ipynb"> Solution CNN1  without centering</a>|
			      			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/08_cnn2_mnist_solution.ipynb">Solution CNN2  MNIST</a>
</li>

		
				      		<li>
      			 09 and 10 Homework: 8 Faces
			<a href="https://www.dropbox.com/sh/oek6lcshf9ws8o4/AAB5hSpN328raDkbdYHH_YsQa?dl=0&preview=8_faces_dataoverview.html"> Data overview</a>|
			 <a href="exercises/09_10_8_faces">Exercise </a>|
			       			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/09_8_faces_only_fc_solution.ipynb"> FC Solution</a>|
						      			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/10_8_faces_cnn_solution.ipynb"> CNN Solution</a>
			
      		</li>
		

		
         </ul>
      </td>
    </tr>

<!-- Woche -->
    <tr>
      <td>5</td>
      <td> 
      		<b>Convolutional Neural Networks II</b> <a href="https://www.dropbox.com/s/p43uvk46hom9zhw/DL-day5-presented.pdf?dl=1">slides</a>
      		<ul>
   					<li>Typical CNN architectures</li>
					<li>Transfer learning: Use pretrained nets for fine-tuning or feature generator</li>
					<li>Feature/activation maps in detail</li>
					<li>Understand CNN features</li>
      					
      					
      		</ul>
      </td>
      <td> 
        <ul>
	<li>
	<a href="https://transcranial.github.io/keras-js/#/mnist-cnn">live CNN in browser</a>
	</li>
	<li>
	<a href="http://yosinski.com/deepvis">Understanding CNNs through visualization</a>
	</li>

	<li>
	<a href="http://cs231n.github.io/understanding-cnn/">cs231 on visualization CNNs</a>
	</li>
	<li>
	<a href="https://blog.keras.io/category/demo.html">Use keras to visualize which image features activate a feature map</a>
	</li>

        </ul>
      </td>
      <td>
      	<ul>
		      		<li> 11 finger-exercise CNN
			<a href="https://www.dropbox.com/s/96a0a0umk3f7xew/11-finger-exercise.pdf?dl=1"> Exercise</a>|
			<a href="https://www.dropbox.com/s/teto11w8awxkj9i/11-finger-exercise-solution.pdf?dl=1"> Solution </a> 
	
      		</li>
	

      		
				  <li> 12 transfer learning<a href="exercises/12_8_faces_fine_tuning"> Exercises</a> | 
      			
	<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/12_8_faces_fine_tuning_solution.ipynb">Solution</a>
	<li>
      			13a optimized image<a href="https://www.dropbox.com/s/956jxouq0eqisn8/13-exercises-optimized-image.pdf?dl=1"> Exercise</a>|
			<a href="https://www.dropbox.com/s/5zyntjgff9k5cgm/13-exercises-optimized-image-solution.pdf?dl=1">Solution</a>|
	      			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/13-optimize-image.ipynb"> Notebook</a>
			</li>
			
			<li>13b adversarial example<a href="https://www.dropbox.com/s/sf8k96kxinknzfh/14-adversarial-example.pdf?dl=1"> Exercises</a> |
			      			<a href="https://www.dropbox.com/s/8cgm7cvr1lcqfsd/14-adversarial-example-solution.pdf?dl=1">Solution</a>
      		</li>


		
 <!-- Woche -->
     <tr>
      <td>6</td>
      <td> 
      		<b>Recurent Neural Networks</b> <a href="https://www.dropbox.com/s/45yfkcacxggdlcu/lecture06.pdf?dl=1">slides</a>
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

          <li><a href="http://www.deeplearningbook.org/contents/rnn.html">DL-book chapter 10 </a></li>


        </ul>
      </td>
      <td>
      	<ul>
      		<li>
			14 Simple RNN:<a href="exercises/14_rnn_simple"> Exercises</a> | 
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/14_simple_rnn_tf1_no_solution.ipynb"> Notebook</a> |
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/14_simple_rnn_tf1_solution.ipynb"> Solution</a>
	
      		</li>
      		<li>
		15 Char RNN <a href="exercises/15_rnn"> Exercise</a> |
		<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/15_char_rnn_didactic_prediction_solution.ipynb"> Notebook</a> 
		
      		</li> 
      		
         </ul>
      </td>
    </tr>

    <!-- Woche -->
    <tr>
      <td>7</td>
      <td> 
      		<b>Un- and Semi-supervised Learning I</b> <a href="https://www.dropbox.com/s/x33aydj6ehyl15t/DL-day7-presented.pdf?dl=1">slides</a>
      		<ul>
   					<li>How to do unsupervised feature learning or representation learning?</li>
					<li>Autoencoder and denoising AE</li>
					<li>Use unsupervised learned features for pattern recognition</li>
					<li>Use unsupervised learned features for classifcation with few labeled instances</li>
      					
       		</ul>
      </td>
      <td> 
        <ul>
	<li>
      			<a href="https://www.dropbox.com/s/dvq5upb5nof090x/Bengio2014-representation-learning.pdf?dl=1">Bengio's Review on representation learning</a>
      		</li>

        </ul>
      </td>
      <td>
      	<ul>
      		<li>
		
		
					16 FC and CNN Autoencoders:<a href="exercises/16_fc_cnn_denoising_autoencoder"> Exercises</a> | 

			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/16_fc_cnn_denoising_autoencoder_solution.ipynb"> Solution</a>
	
		
			
      		</li>

      		<li>
		
					17 Using unsupervised learned featurs for classification:<a href="exercises/17_MNIST_feature_evaluation"> Exercises</a> | 
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/17_MNIST_feature_evaluation.ipynb"> Notebook</a> |
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/17_MNIST_feature_evaluation_solution.ipynb"> Solution</a>

      		</li>
         </ul>
      </td>
    </tr>
       <!-- Woche -->
    <tr>
      <td>8</td>
            
      <td> 
      <b>Un- and Semi-supervised Learning II</b> <a href="https://www.dropbox.com/s/yyw0vuvfnnlz8e6/DL-day8-presented.pdf?dl=1">slides</a>
      		
      		<ul>
   					<li>Classical and denoising AE</li>
					<li>Classical and denoising variational AE</li>
					<li>Ladder network for un- and semi-supervised learning</li>
					<li>Spotlight talks</li>
					<li>Poster presentations</li>
      					
       		</ul>
      </td>
      <td> 
        <ul>
	<li>
        DL-book chapter 14
	</li>
	<li>
	<a href="https://www.youtube.com/watch?v=ZlyqNiPFu2s">The ladder network presented by its inverntor H. Valpola</a>
	</li>

        </ul>
      </td>
      <td>
      	<ul>


      		<li>
					18 Using a Variational autoencoder to generate digit examples:<a href="exercises/18_VAE"> Exercises</a> | 
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/18_VAE.ipynb"> Notebook</a> |
			<a href="https://github.com/tensorchiefs/dl_course/blob/master/notebooks/18_VAE_solution.ipynb"> Solution</a>

      		</li>
         </ul>
      </td>
    </tr>
   
 






