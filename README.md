# SRCNN (Super-Resolution Convolutional Neural Network)

There are many ways to upscale an image like:
- Nearest Neighbour Interpolation
- Bilinear Interpolation
- BiCubic Interpolation
- SRCNN

Upscaling methods such as **nearest-neighbor, bilinear, and
bicubic interpolation** are purely mathematical techniques. They estimate
new pixel values using fixed formulas based on surrounding pixels.
Although these methods are fast, they often produce **blurry images**
because they cannot recover lost high-frequency details or textures.

## SRCNN

SRCNN is an early deep learning model proposed for image super-resolution.
Its objective is to reconstruct a high-resolution image from a
low-resolution input using a convolutional neural network.

SRCNN improves upon these approaches by **learning the upscaling process
from data instead of fixed mathematical rules**. The low-resolution image
is first upscaled using bicubic interpolation and then passed through a
CNN that learns how to sharpen edges and restore fine image details.

The SRCNN architecture consists only of convolutional layers and follows
three main stages:
1. feature extraction from the upscaled image,
2. non-linear mapping between low- and high-resolution features,
3. reconstruction of the final high-resolution image.

This learning-based approach allows the
model to generate visually sharper and more accurate results compared to
traditional interpolation methods.

SRCNN is simple but significant, as it demonstrated that convolutional
neural networks can outperform classical mathematical methods in image
restoration tasks. It serves as a foundation for many modern
super-resolution and image deblurring techniques.

### FSRCNN (Fast Super-Resolution Convolutional Neural Network)

FSRCNN is an improved and faster version of SRCNN designed for image
super-resolution. While SRCNN applies convolution on an already
upscaled image, FSRCNN works directly on the **low-resolution input**,
making it significantly more efficient.

Instead of first enlarging the image using interpolation, FSRCNN learns
to extract features in the low-resolution space and performs upscaling
only at the final stage using a deconvolution (transposed convolution)
layer. This design reduces computation and speeds up both training and
inference.

The FSRCNN architecture is deeper than SRCNN but uses smaller filter
sizes and fewer parameters. It consists of feature extraction,
shrinking, non-linear mapping, expanding, and upsampling stages, each
designed to balance speed and reconstruction quality.

FSRCNN achieves comparable or better image quality than SRCNN while
being much faster.

