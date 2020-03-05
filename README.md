## The Artificial Hebbian Neuronal Network:  

### Introduction: 
The following project is an attempt to create a artificial neural network that can be trained using Hebbian principles. 

My goal for this project is threefold: 
 1. To create a network that can be infinitely grown to learn new patterns of data without re-training the entire network. 
 2. To create a network that has the ability to track the age of each learned pattern. 
 3. To be biologically plausible by not requiring backpropagation, or gradient descent. 

To do this, I have created two classes, one is the hebbianNeuron(), while the other is hebbianLayer() which encapsulates the hebbianNeuron class. 


## Each Hebbian Neuron: 
Each hebbian neuron when initialized will generate random connections to the previous layer, and store a pattern of activation which the neuron will recognize. 

The way the neuron will recognize the pattern of activation is through a simple MSE function. If the input pattern and the stored pattern produces less than a specified amount of error the neuron will output a value of 1.0 * neuron weight. 

