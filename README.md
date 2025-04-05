# Virus-MNIST-Classification
Developed a malware image classification model using MobileNetV2, achieving 59% accuracy on a dataset of 48,422 training and 3,458 testing images across 10 virus classes. This project leveraged transfer learning to efficiently classify malware images with minimal computational resources.


Project Overview

This project focuses on classifying malware images from the Virus MNIST dataset using transfer learning with MobileNetV2. The dataset consists of 48,422 training images and 3,458 testing images, each categorized into one of 10 malware classes.

Key Features

Dataset Preprocessing:

Resized images to 32x32 pixels.

Converted grayscale images to RGB.

Normalized pixel values to enhance model performance.

Model Architecture:

Utilized MobileNetV2 with pre-trained ImageNet weights, excluding the top classification layer.

Added a GlobalAveragePooling2D layer followed by a Dense layer with 10 units and sigmoid activation to match the 10-class classification task.

Compilation and Training:

Compiled the model using the Adam optimizer with a learning rate of 0.001 and sparse categorical cross-entropy loss.

Trained for 10 epochs, achieving approximately 60% accuracy on the training set and 59% on the validation set.

Test Performance:

Evaluated the model on the test set, achieving an accuracy of approximately 59%.

Code Structure

Data Preparation: Scripts for loading, preprocessing, and splitting the dataset.

Model Definition: Code for defining the MobileNetV2 architecture with custom layers.

Training and Evaluation: Scripts for training the model and evaluating its performance on validation and test sets.
