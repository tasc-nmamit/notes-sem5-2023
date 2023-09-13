5 Sept 2023

# Definition
Deep Learning is a subset of a more general field of AI called ML, which is predicated on this idea of **learning from example**.

---

# The neuron-human brain (Analogy for Deep Learning)

(6m MSE, 10m SEE)

- The foundational unit of the human brain is the **neuron**.
- The neuron receives its inputs along antennae like structure called **dendrites**.
	- Each of the incoming connections are dynamically strengthened or weakened based on how often it is used.
- After being weighted by the strength of their respective connections, the inputs are summed together in the **cell body**.
	- 

![[Neurons.png|450]]

- Dendrites
- Cell body
- Axon 
- Synaptic terminal

Inputs -> Strengths -> Sum & Transform -> Output

---

# Artificial Neuron

Artificial Neuron is a mathematical function based on a model of biological neurons, where each neuron takes inputs, weighs them separately, sums them up and passes this sum through a nonlinear function to produce output.

![[Artificial Neuron.png]]

---
# What is a perceptron?

(10m - Explain perceptron and it's working.)

Perceptron is a building block of an artificial neural network. It is also understood as an Artificial Neuron or NN Unit that helps detect certain data computations.

## Basic Components of Perceptron

![[Perceptron.png]]

## Working

- A weight is assigned to every input. 
- Net input function (weights + bias) -> The weighted inputs are summed.
	- Bias can be considered as the line of intercept in a linear equation : $y = mx + c$ 
	- (c is the bias)
- Activation function -> Activate if certain criteria are met (i.e imp signals are present)
- Output

ps. Perceptron -> no hidden layers

6 September 2023
# Working of Perceptron

Perceptron is consider a single-layer neural network
- 4 Parameters → input values, weights & bias, net sum and activation function

## Step 1: Weighted Sum
Multiply all input values with corresponding weight values and calculate the weighted sum.
$$
\Sigma (wi*xi) = x1*w1 + x2*w2 + ... + wn*xn
$$
Activation function → converts the signal to lineararity format or non-lineararity format  
for this we need bias?
$$
\Sigma (wi*xi) + b
$$
FAQ → Why do we need bias?

## Step 2: Activation function

An activation function is applied with the above-mentioned weighted sum, which gives us output either in binary format or a continuous value as follow. (there are different types of activation function with different formulas which will be studied in the later classes)
$$
Y = f(\Sigma wi*xi + b)
$$

---

# Multilayer Perceptron

There is an additional hidden layer. And there is backward propagation of error...

- Forward Stage
- Backward Stage

---
7 Sep 2023
# Activation function 

Q. Explain activation function with examples.  
Q. Differentiate between sigmoid and relu.  
Q. Explain dead relu problem and how it can be overcome with the help of leaky relu.  
Q. explain vanishing gradient problem with an example.  
Q. Explain exploding gradient problem with an example.

**Definition**: It is the internal state of the neuron. It represents is used to convert the input signal of ANN node to an output signal.

It is applied to the weighted sum of inputs and biases of the neuron.

- It introduces the non linearity to the output of individual neurons or artificial neurons.
- Decides whether a neuron should be activated or not based on input signals and weights

ps. Linearity vs non-linearity in this context  
Without the activation function, the output will be linear ($\Sigma wi*xi$). Activation function makes it non linear by applying say sigmoid function etc...

![[Activation functions.png]]

## Linear activation function

Type of activation function, which outputs a linear combination of input values.
- It is the simplest activation function and is knowns as the identity function.

Formula : $f(x) = x$

In an ideal system, activation function would be linear.

- It is unable to learn complex relationship between input features.
- Typically used in regression problems.

> [!calculation]-  
> For exam, draw any NN (with say a few hidden layers and finally the output) of your choice and explain the activation function.  
> ![[Perceptron.png|500]]
>
> Apply Linear activation function on the input. Take 3 inputs $x1,\ x2\ and\ x3$  
> 	Step 1: calculate weighted sum + bias  
> 	Step 2: Apply Linear AF $f(x) = x$
>
>Now the apply the same for hidden layers....  
>Finally do this until you get the output.  
>![[NN with 1 hidden layer.png|400]]  
>![[NN with 1 hidden layer 2.png|400]]

## Sigmoid activation function

It is an activation function which squishes the input to an output between 0 and 1.

- Used for classification function (in the final output layer)
- (ps. can't be used for regression)
- It's not recommended to use in the hidden layers. Why? (vanishing and exploding gradient problem?)

Formula for sigmoid function → 
$$ 
f(x) =  \frac{\mathrm{1} }{\mathrm{1} + e^{-x} } 
$$

![[Sigmoid function.png]]

>[!calculate]-  
>Calculation of output using sigmoid activation function - refer notes and insert photo
>

## Relu Activation Function

Formula: $f(x) = max(0, x)$  
![[Relu activation function graph.png]]

- Computationally fast
- Eliminates the problems such as vanishing and exploding gradient in sigmoid activation function
- Problem with ReLu is dead ReLu

## Tanh activation function (Hyperbolic tangent)

Formula: 
$$
f(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}
$$
where e = Euler's number $\approxeq$ 2.71828

## Leaky ReLu

Formula: $f(x) = max(ax, x)$

It is the variation of the standard ReLu activation function that addresses some of the limitation of the ReLu function such as 'dying ReLu' problem.


---

# Forward & Backward propagation #imp #10m

>[!diagram]  
>Consider the following NN (notebook)

## Forward Propagation 
- get the inputs, calculate weighted sum, add bias & activation function and find the output

## Backward Propagation (of errors)
- It is the method of fine tuning the weights of a neural network based on the error or loss obtained in the feed forward network.

Consists of 2 steps

- $y = w^Tx + b$

### 1. Weight Updation Formula
- $w_{new} = w_{old} - \eta\frac{\partial L}{\partial w_{old}}$
- where $\eta$ is learning rate (a small value say 0.001)
- $\frac{\partial L}{\partial w_{old}}$ is the slope
- 
- Gradient descent...
	- 

### 2. Chain rule of differentiation


---
