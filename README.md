# Week 1
## Neural Networks and Deep Learning
The first week consisted of learning about Neural Networks and Deep Learning and then writing a code of a model which recognises handwritten digits of the MNIST Dataset.

A neural network is an machine learninng model which resembles the human brain to recognise patterns by tuning the weights and biases by back propagation.



## Model Architecture
The hyperparameters of the model are listed below

Dataset:MNIST

Learning Rate:0.001

Epochs:15

Optimiser:Adam

Loss:Cross Entropy Loss

Input size:784 (28 by 28 images)

Output classes: 10 (10 digits)

The model is a fully connected neural network with the following layer
configuration:

784 → 256 → 64 → 10

The input layer consists of 784 features (corresponding to a flattened
28×28 image), followed by two hidden layers with 256 and 64 neurons
respectively, and an output layer with 10 neurons representing the
target classes.

Final Accuracy: 98.36%
