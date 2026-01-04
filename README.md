# Week 1
## Neural Networks and Deep Learning
The first week consisted of learning about Neural Networks and Deep Learning and then writing a code of a model which recognises handwritten digits of the MNIST Dataset.

A neural network is an machine learninng model which resembles the human brain to recognise patterns by tuning the weights and biases by back propagation.



## Model Architecture
The hyperparameters of the model are listed below

- Dataset:MNIST
- Learning Rate:0.001
- Epochs:15
- Optimiser:Adam
- Loss:Cross Entropy Loss
- Input size:784 (28 by 28 images)
- Output classes: 10 (10 digits)

The model is a fully connected neural network with the following layer
configuration:

784 → 256 → 64 → 10

The input layer consists of 784 features (corresponding to a flattened
28×28 image), followed by two hidden layers with 256 and 64 neurons
respectively, and an output layer with 10 neurons representing the
target classes.

Final Accuracy: 98.36%

This model uses only fully connected layers to recognise the digit so it fails in most of the practical cases

This image which is written on a piece of paper by me (compressed later to 28 * 28) is recognised by the model as 5

This might be due to various reasons like the digit not being centred, the texture of the page etc.
<img width="934" height="934" alt="image" src="https://github.com/user-attachments/assets/beedda28-3243-4159-b3f2-b0b4a2080ad8" />

Later I tested it with this image
<img width="28" height="28" alt="image" src="https://github.com/user-attachments/assets/be4b9699-d5d4-4784-b561-445815512872" />
Which gave the result as 6

This is due to the fact that MNIST Dataset contains images in grayscale but has different shades for every pixel but this image ha only black and white pixels.

