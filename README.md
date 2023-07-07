# Convolutional Autoencoder (CAE) vs. Fully Connected Autoencoder (FCAE) Comparison

This repository provides code and instructions for comparing the performance of Convolutional Autoencoder (CAE) and Fully Connected Autoencoder (FCAE) in reconstructing images using the MNIST dataset. The results demonstrate that the CAE outperforms the FCAE due to the presence of convolutional layers, resulting in clearer and higher-resolution reconstructed images.

## Dataset

The dataset used for this comparison is the MNIST dataset, which consists of 60,000 training images and 10,000 test images of handwritten digits. The images are grayscale and have a resolution of 28x28 pixels. The dataset is widely used for training and evaluating machine learning models in the field of computer vision.

To use the MNIST dataset for the experiments, please download it from the official MNIST website or any other reliable source. Make sure to follow the instructions provided with the dataset to prepare it for training the autoencoders.

## Implementation

### Convolutional Autoencoder (CAE)

The CAE implementation includes the following steps:

1. **Step 1**: Data Preparation

   - Download the MNIST dataset and preprocess it by normalizing the pixel values to the range [0, 1].
   - Split the dataset into training and test sets.

2. **Step 2**: Model Architecture

   - Build the CAE model using convolutional and pooling layers for the encoder, and upsampling and convolutional layers for the decoder.
   - Define the loss function and optimization algorithm for training the CAE.

3. **Step 3**: Model Training

   - Train the CAE on the training set using the defined loss function and optimization algorithm.
   - Monitor the training process and evaluate the performance on the validation set.

4. **Step 4**: Image Reconstruction

   - Use the trained CAE to reconstruct images from the test set.
   - Compare the reconstructed images with the original images to assess the quality of reconstruction.

### Fully Connected Autoencoder (FCAE)

The FCAE implementation follows a similar structure to the CAE, but without the convolutional and pooling layers. Instead, it uses fully connected layers for both the encoder and decoder. This serves as a baseline for comparison with the CAE.

The steps for implementing and evaluating the FCAE are the same as those for the CAE, but with a different model architecture.

