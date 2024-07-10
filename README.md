# Dog Heart Classification Using Convolutional Neural Networks

## Overview

This repository contains the implementation of various Convolutional Neural Network (CNN) architectures for the classification of dog heart sizes from X-ray images. The models leverage residual blocks and Inception modules to enhance feature extraction capabilities and improve classification accuracy.

## Models Implemented

1. **CNN\_V0**
   - Baseline CNN model with five convolutional layers followed by max-pooling.
   - Three fully connected layers for classification.

2. **CNN\_V1**
   - Enhanced CNN model incorporating residual blocks to improve learning and generalization.
   - Same architecture as CNN\_V0 with additional residual connections.

3. **CNN\_V2**
   - CNN model with Inception modules to capture multi-scale features.
   - Replaces standard convolutional layers with Inception modules for blocks 2 to 5.

## Dataset

The dataset used in this project consists of X-ray images collected from Shanghai Aichong Pet Hospital. The dataset includes images labeled as 'Large', 'Normal', and 'Small' based on the heart size. The dataset is divided into training, validation, and test sets as follows:

| Dataset    | Large | Normal | Small | Total |
|------------|-------|--------|-------|-------|
| Training   | 619   | 573    | 208   | 1400  |
| Validation | 76    | 91     | 33    | 200   |
| Test       | 175   | 163    | 62    | 400   |

## Results

The performance of different models is summarized below:

| Model    | Accuracy |
|----------|----------|
| VGG16    | 0.79     |
| CNN\_V0  | 0.6875   |
| CNN\_V1  | 0.7525   |
| CNN\_V2  | 0.6625   |


## Testing
The `model_weights` directory contains the saved weights of the three models, and the `test_csv_file` directory contains the prediction results on the test set.
To test the accuracy, please refer to https://github.com/YoushanZhang/Dog-Cardiomegaly.git

