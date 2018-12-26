# NEURAL-NETWORKKS

## BACKGROUND

A neural network can be thought of as a network of “neurons” which are organised in layers. similar to the way neurons are connected to each other in brain, a neural network takes an input, passes it through a function based on which certain neurons get excited and further based on which certain output is produced.  The predictors (or inputs) form the bottom layer, and the forecasts (or outputs) form the top layer. There may also be intermediate layers containing “hidden neurons”.

---

## Structure of a Neural Network
![1 6xj691fpwf3s-mwucbxsjg](https://user-images.githubusercontent.com/45025357/50448792-289ab180-0949-11e9-81f8-9bc7e6700351.jpeg)

   The *circle* represnts *Neurons* and *line* represents *Synapses*. Synapses takes the input and multiply it bya weight. Neurons add he outputs from all the synapses and apply an activation Fucntion. 

* **Input Layer:**   Number of neurons in this layer corresponds to the number of inputs to the neuronal network. This layer  do not take part in the actual signal modification, but only transmits the signal to the following layer. 
   
* **Hidden Layer:** This layer has arbitrary number of layers with arbitrary number of neurons. The nodes in this layer take part in the signal modification, hence, they are active.

* **Output Layer:** The number of neurons in the output layer corresponds to the number of the output values of the neural network. The nodes in this layer are active ones.

* Typically in a binary dependent variable, there is only one node in the output layer(output as 1 or 0)

* Having more than more 1 hidden layer helps in achieving hign non linearity.

---

## Key steps in Neural Network:
 Training a neural network basically means calibrating of all the weights by repeating two key steps, forward propation and backward propagation. 
 
 **1. Forward Propagation:** 
   We apply a set of weights to the input data and calculate an output. For the first forward propogation, the set of weights is selected randomly.  we sum the products of the inputs with their corresponding set of weights to arrive at the first values for the hidden layer and then apply the activation Function for it.
     Most used activation functions are:
      * Linear activation Function - *for regression*
      * unit step activation Function - *for classification*
      * Sigmoid activation Function - *for classification*
      * Tan Hyperbolic activation Function 
      * ReLu activation Function - *most commonly used*
      * Softmax activation Function - *Multiclass classification*
     
  After aplying one of the activation function, the final output is calculated. Because we used a random set of initial weights, the value of output neuron is off the mark. If the process is stopped here, this set of weights would be a inaccurate  neural network. 
  
 **2. Backward Propagation**
    To improve the model, first we have to quantify just how wrong our predictions are. Then, adjust the weights accordingly so that the margin of error are decreased. Similar to forward propagation, back propagation calculations occur at each *layer*.
       output sum margin of error = *target - calculated*
 * ***Forward prop helps in estimating the error, while backward prop helps in reducing the error.***  
 
---      
### Learning methods
* Artificial neural networks work through the optimized weight values.
* The method by which the optimized weight values are attained is called learning
* In the learning process  try to teach the network how to produce the output when the corresponding input is presented
* When learning is complete: the trained neural network, with the updated optimal weights, should be able to produce the output within desired accuracy corresponding to an input pattern.
Learning methods
* *Supervised learning*
* *Unsupervised learning*
* *Reinforced learning*


![screen shot 2018-12-26 at 7 43 59 pm](https://user-images.githubusercontent.com/45025357/50451171-6ce17e00-0958-11e9-95e9-212f249d900f.jpg)


###  *Important terminology* 
* Typically one pass of forward & one backward propagation constitues an ** *Epoch* ** . more the number of epochs, more is the time weight is adjusted. 
* The number of training examples considered per epoch is called as ** *Batch Size* **
* The process in which backward propagation works is often referred as ** *Chain Rule* **

###  ANN applications
* Classification, the aim is to predict the class of an input vector
*  Pattern matching, the aim is to produce a pattern best associated with a
given input vector
* Pattern completion, the aim is to complete the missing parts of a given input vector
* Optimization, the aim is to find the optimal values of parameters in an optimization problem
* Control, an appropriate action is suggested based on given an input vectors
* Function approximation/times series modeling, the aim is to learn the functional relationships between input and desired output vectors;
* Data mining, with the aim of discovering hidden patterns from data (knowledge discovery)

