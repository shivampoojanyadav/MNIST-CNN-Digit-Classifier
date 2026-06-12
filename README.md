# MNIST CNN Digit Classifier

## Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify handwritten digits from the MNIST dataset.

The model is trained on grayscale images of handwritten digits (0–9) and learns to recognize and classify unseen digit images with high accuracy.

## Features

* Built using PyTorch
* Uses Convolutional Neural Networks (CNNs)
* Trained on the MNIST dataset
* Supports GPU acceleration (CUDA) when available
* Evaluates model performance on test data
* Saves the trained model for future use
* Predicts handwritten digit classes (0–9)

## Dataset

The project uses the MNIST dataset provided through TorchVision.

* 60,000 training images
* 10,000 testing images
* Image size: 28 × 28 pixels
* 10 digit classes (0–9)

## Model Architecture

### Feature Extraction Layers

* Conv2D (1 → 8 channels)
* ReLU Activation
* Max Pooling
* Conv2D (8 → 16 channels)
* ReLU Activation
* Max Pooling

### Classification Layers

* Fully Connected Layer (16 × 7 × 7 → 64)
* ReLU Activation
* Fully Connected Layer (64 → 10)

## Technologies Used

* Python
* PyTorch
* TorchVision
* NumPy
* Matplotlib

## Training Process

1. Load and preprocess the MNIST dataset
2. Create DataLoaders for batching
3. Train the CNN using CrossEntropyLoss
4. Optimize weights using Adam Optimizer
5. Evaluate performance on the test dataset
6. Save the trained model

## Results

The model successfully learns handwritten digit patterns and achieves strong classification performance on unseen test images.

## How to Run

1. Clone the repository

```bash
git clone <repository-url>
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the Jupyter Notebook

```bash
CNN_Vision_project.ipynb
```

## Future Improvements

* Add confusion matrix visualization
* Display misclassified images
* Experiment with deeper CNN architectures
* Build a Streamlit web application for digit prediction

## Author

Shivam Poojan Yadav
