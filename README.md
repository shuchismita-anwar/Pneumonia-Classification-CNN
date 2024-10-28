# Pneumonia Classification using CNN on PneumoniaMNIST

This repository provides a convolutional neural network (CNN) model to classify chest X-ray images as either pneumonia or normal cases, using the PneumoniaMNIST dataset from the MedMNIST collection. The code handles dataset loading, model training, and evaluation, providing key metrics to assess model performance.

## Dataset
[PneumoniaMNIST](https://medmnist.com/) is a dataset designed for binary classification of pneumonia in chest X-rays. The dataset is split as follows:
- **Train Set**: 4708 samples
- **Validation Set**: 524 samples
- **Test Set**: 624 samples

The images are grayscale, resized, and normalized for input into the CNN model.

## Model Architecture
The CNN model is implemented using PyTorch with the following structure:
1. **Convolutional Layer 1**: 32 filters, 3x3 kernel, ReLU activation
2. **Max Pooling Layer 1**: 2x2
3. **Convolutional Layer 2**: 64 filters, 3x3 kernel, ReLU activation
4. **Max Pooling Layer 2**: 2x2
5. **Convolutional Layer 3**: 128 filters, 3x3 kernel, ReLU activation
6. **Max Pooling Layer 3**: 2x2
7. **Fully Connected Layer**: 128 neurons
8. **Output Layer**: 2 neurons for binary classification

## Requirements
- Python 3.x
- numpy
- torch
- scikit-learn
- medmnist

To install requirements:
```bash
pip install numpy torch scikit-learn medmnist
