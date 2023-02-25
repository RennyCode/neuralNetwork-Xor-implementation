## neuralNetwork-Xor_implementation
This project has two parts, the first notebook is a demonstration of a manually build of a Perceptron (a Neural Network which consists of BTU activations) with a single hidden layer.

The second notebook contains the same network demonstration with training.



<div style = "padding-bottom: 150; padding-top: 150;">
  <p align="center">
    <img src="/pic1.png"  style = " height: 250;  display:block; width:50%;"/>
   </p>
</div>



## Workflow
the goal is to demonstrate how a simple neural network can implement a Xor Gate,

reminder - a Xor Gate is a binary function that receives two binary inputs, if they are equal then the output is equal to '0' otherwise '1'.

In the first part, we simply build a network and tuned the weight values to show how it can implement the Xor function.

In the secod, part we demonstrated how the network can actually learn the right values of the weights to produce the right output by the use of gradient descent.


## A Short shot of theory (simplification)
The basic idea is to build a network that can supplement the Xor Function, to do that we must take all the possible input combination and assure that each one will provide the right output in our network.

The forward calculation between layers of the network is a matrix multiplication, and an activation function on each value of the results, the BTU activation is suitable for this case since we are working in the Binary terms.

Each neuron has his own bias value that acts as a threshold

The Math: 

Z = WX^t + b

y = BTU(Z)

After the calculation we get a final result, the training is the implementation of change in the weight values of the network based on that result.
We decide on a loss function to measure the error and implement changes to the weights, so the loss value will go lower, and by that getting closer to a right prediction for the values of our input.

It should be mentioned that not all networks can implement all functions, but we could follow a logic on how to build a network to match our function that we're trying to implement:

If we have n inputs and 2^n hidden units in our hidden layer we could provide a simple solution, in a way that each hidden unit represents a single combination, in practice we can't clearly assume that units get that type of responsibility, but as long as the solution is provided in the legal range of solutions it doesn't make a difference.



