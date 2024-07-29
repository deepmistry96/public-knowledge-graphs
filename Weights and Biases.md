#lowlevel 


[[Weights]] and [[biases]] are neural network [[parameters]] that simplify machine learning data identification.

The weights and biases develop how a neural network propels data flow forward through the network; this is called [forward propagation](https://h2o.ai/wiki/forward-propagation). Once forward propagation is completed, the neural network will then refine connections using the errors that emerged in forward propagation. Then, the flow will reverse to go through layers and identify nodes and connections that require adjusting ; this is referred to as [backward propagation](https://h2o.ai/wiki/backpropagation).

**Weights** refer to connection managements between two basic units within a neural network.

To train these units to move forward in the network, weights of unit signals must be increased or decreased. These connections will then be tested, reversed through the network to identify errors, and repeated to produce the optimal results.

**Biases** in neural networks are additional crucial units in sending data to the correct end unit. Biases are units entirely separate from the units already in place within the network. They are added to the middle data units to help influence the end product. Biases cannot be added to initial units of data. Like weights, biases will also be adjusted through reversing the neural network flow in order to produce the most accurate end result. When a bias is added, even if the previous unit has a value of zero, the bias will activate a signal and push the data forward.



## Terms Related to Weights and Biases

**Neuron** - Basic units of the neural network containing individual data features.

**Layers** - A collection of unrelated neurons (the input layer) that connect to another set of neurons. This continues until the final layer of neurons (the output layer) is reached. Weights affect the neuron connections between layers.

**Hidden Layers** - Layers between input layers and output layers. This is where artificial neurons take in a set of weighted inputs and produce an output through an [activation function](https://h2o.ai/wiki/activation-function).


### **Activation and Loss Functions**

**Activation Function** is the output of an input. The data from a neuron in a previous layer will produce a similar value in the next layer.

**Loss Function** is the difference between the expected algorithm output and the actual output. The loss, or error, is a measurement for how off the algorithm is compared to the predictions.

**Regularization** - A technique that narrows down the connection weights. The weight values may become too large and unusable. Regularization brings the weights back down to a manageable value which will optimize the model's functionality.

**Parameters** - The weights and biases of neuron connections.

**Value** - Bias introduces a value of 1 to the hidden layers. Changing the value of the activation function to a 1 directs the neural network to a more optimal product. Adding value to hidden layers teaches the machine learning model how data produced by the input layer must be used.

## Why are Weights and Biases Important?

Weights and biases are crucial concepts to a neural network. The neural network processes the characteristics of a data subject (like an image or audio clip) and produces an identification of the subject.

- Weights set the standards for the neuron’s signal strength. This value will determine the influence input data has on the output product.
    
- Biases give extra characteristics with a value of 1 that the neural network did not previously have. The neural network needs that extra information to efficiently propagate forward.
    
- Weights and biases both better distinguish the neurons and their connections to give an accurate output.