## SRCNN (Super-Resolution Convolutional Neural Network)

SRCNN is an early deep learning model proposed for image super-resolution.
Its objective is to reconstruct a high-resolution image from a
low-resolution input using a convolutional neural network.

Traditional upscaling methods such as **nearest-neighbor, bilinear, and
bicubic interpolation** are purely mathematical techniques. They estimate
new pixel values using fixed formulas based on surrounding pixels.
Although these methods are fast, they often produce **blurry images**
because they cannot recover lost high-frequency details or textures.

SRCNN improves upon these approaches by **learning the upscaling process
from data instead of fixed mathematical rules**. The low-resolution image
is first upscaled using bicubic interpolation and then passed through a
CNN that learns how to sharpen edges and restore fine image details.

The SRCNN architecture consists only of convolutional layers and follows
three main stages: feature extraction from the upscaled image, non-linear
mapping between low- and high-resolution features, and reconstruction of
the final high-resolution image. This learning-based approach allows the
model to generate visually sharper and more accurate results compared to
traditional interpolation methods.

SRCNN is simple but significant, as it demonstrated that convolutional
neural networks can outperform classical mathematical methods in image
restoration tasks. It serves as a foundation for many modern
super-resolution and image deblurring techniques.
