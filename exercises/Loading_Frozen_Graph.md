## Loading Frozen Graph

a) Open the notebook [Loading_Frozen_Graph](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/Loading_Frozen_Graph.ipynb) and run the fist 2 cells to load the "art style transfer" graph.

b) Now read in an image of yourself or some random image(cat, dog, etc.). Replace "bigstock-Standard-Poodle-7733433.jpg" with the name of your image.

c) Visualize the graph in Tensorboard. Look at the names of the nodes.

d) Modify cell 10 with the right name of the input node and feed your image through the graph.

Hint: TensorFlow names operation with n tensor outputs by default "op_name:0", "op_name:1", ... "op_name:n-1"

e) Optional: Real time art transfer. Write a loop that takes images with your webcam and feeds the images through the graph.
