# Week 2

## Convolutionary Neural Network

This week's learning is about Convolutionary Neural Network and then building a CNN model using Pytorch.

A Convolutional Neural Network (CNN) is a type of neural network designed for image data which uses a combination of Convolutionary layers, Pooling and Fully Connected layers to produce an output. 
Instead of connecting every input to every neuron, a CNN uses convolutions to automatically learn spatial features like edges, textures, and shapes.

## Model Configuration

The following hyperparameters were used to define and train the CNN model:

- **Input channels:** 3 (RGB images)
- **Number of output classes:** 10
- **First convolution output channels:** 16
- **Second convolution output channels:** 32
- **Learning rate:** 0.001
- **Number of epochs:** 10

---

## Model Architecture

The model is trained on the CIFAR-10 Dataset.

The model is a Convolutional Neural Network (CNN) with the following structure:

- **Convolutional Layers:** Two convolutional layers with 3×3 kernels and
  16 and 32 output channels are used to extract spatial features from the
  input images.
- **Normalization and Activation:** Each convolutional layer is followed
  by Batch Normalization and ReLU activation to improve training
  stability.
- **Pooling Layers:** Max Pooling layers reduce the spatial dimensions
  after each convolution block.
- **Fully Connected Layers:** The extracted features are flattened and
  passed through a fully connected layer with 128 neurons.
- **Output Layer:** A final fully connected layer with 10 neurons produces
  class scores for classification.
