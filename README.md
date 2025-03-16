# Convolutional Denoising Autoencoder for CIFAR-10

This repository contains the python notebook for implementation of a **Convolutional Autoencoder** designed to remove noise from CIFAR-10 images. The model is trained using **Keras**

## Features

- **Uses CIFAR-10 dataset** for training and evaluation
- **Adds Gaussian noise** to images to create a noisy dataset
- **Trains a convolutional autoencoder** to reconstruct clean images
- **Includes visualization** of input, noisy, and denoised images

## Model Brief

### Encoder:
- Consists of **three convolutional (Conv2D) layers**, each followed by **BatchNormalization** and **MaxPooling (MaxPool2D)** for feature extraction and dimensionality reduction
- **No dropout** is used in the model, ensuring that all learned features contribute to reconstruction
- **Skip connections** are incorporated to retain and restore essential information lost during convolution and deconvolution, enhancing the quality of the reconstructed images
