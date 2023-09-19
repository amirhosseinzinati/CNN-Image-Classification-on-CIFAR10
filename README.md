# CNN-Image-Classification-on-CIFAR10
This repository contains code for training a convolutional neural network (CNN) on the CIFAR10 dataset using PyTorch. The model achieves 77% accuracy on the test set.

Model Architecture
The CNN model consists of the following layers:

Conv2d (3, 32, kernel_size=3, padding=1)

ReLU

Conv2d (32, 64, kernel_size=3, stride=1, padding=1)

ReLU

MaxPool2d (kernel_size=2, stride=2)

Conv2d (64, 128, kernel_size=3, stride=1, padding=1)

ReLU

Conv2d (128, 128, kernel_size=3, stride=1, padding=1)

ReLU

MaxPool2d (kernel_size=2, stride=2)

Conv2d (128, 256, kernel_size=3, stride=1, padding=1)

ReLU

Conv2d (256, 256, kernel_size=3, stride=1, padding=1)

ReLU

MaxPool2d (kernel_size=2, stride=2

Flatten

Linear (25644, 1024)

ReLU

Linear (1024, 512)

ReLU

Linear (512, 10)

The model is trained for 15 epochs using cross-entropy loss and the Adam optimizer with a learning rate of 0.005.
