## neuralNetwork-Xor_implementation
This project has two parts, the first notebook is a demonstration of a manually build of a Prespectron (a Neural Network which consists of BTU activations) with a single hidden layers.

The seconde notebook contains the same network demonstration with trainning.



<div style = "padding-bottom: 150; padding-top: 150;">
  <p align="center">
    <img src="/pic1.png"  style = " height: 250;  display:block; width:50%;"/>
   </p>
</div>



## Workflow
the goal is to demonstrate how a simple neural network can implement a Xor Gate,

reminder - a Xor Gate is a binary function that recives two binary inputs, if they are equal then output is equal to '0' otherwise '1'.

In the first part we simplly build a network and tunned the weight values to show how it can implement the Xor function.

In the secode part we demonstrated how the network can actually learn the right vaules of the weights to produce the right output by the use of gradient decent.


## A Short shot of theory (simplification)
The basic idea is to build a network that can supplement the Xor Fucntion, to do that we must take all of the possible input combination and assure that each one will provide the right output in our network.

The forward calculation between layers of the network is a matrix multiplication, and a ativation fuction on each value of the results, the BTU activation is sutiable for this case since we are working in the Binary terms.

each neuron has his own bias value that acts as a threshold

the math: 

Z = WX^t + b

y = BTU(Z)

If we have n inputs and 2^n hidden units in our hidden layer we could provide a simple solution, in a way that each hidden unit represents a single combanation, in practice we can't clearly assume that units get that type of responsibility, but as long as the solution is provided in the legal range of solutions it doesn't make a difference.

