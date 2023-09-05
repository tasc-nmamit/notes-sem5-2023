5 Sept 2023

### Definition

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

### Basic Components of Perceptron

![[Perceptron.png]]

### Working

- A weight is assigned to every input. 
- Net input function (weights + bias) -> The weighted inputs are summed.
	- Bias can be considered as the line of intercept in a linear equation : $y = mx + c$ 
	- (c is the bias)
- Activation function -> Activate if certain criteria are met (i.e imp signals are present)
- Output

ps. Perceptron -> no hidden layers


---


Forward & Backward propagation

Equation - $\Sigma$
