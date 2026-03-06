# CNN Image Classification using CIFAR-10

This project implements a Convolutional Neural Network using TensorFlow and Keras to classify images from the CIFAR-10 dataset.

The notebook trains a CNN model, evaluates performance, and visualizes training results.

## Project Objective
Build a CNN model that classifies images into 10 categories from the CIFAR-10 dataset.

Categories include:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

## Tech Stack

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas

## Dataset

CIFAR-10 dataset

Key details

- 60,000 color images
- Image size. 32 × 32 pixels
- 10 object classes
- 50,000 training images
- 10,000 test images

Dataset loads directly using TensorFlow.

## Model Architecture

The CNN architecture includes:

- Convolution Layer  
  - 32 filters  
  - Kernel size 3 × 3  
  - ReLU activation  

- Max Pooling Layer  
  - Pool size 2 × 2  

- Convolution Layer  
  - 64 filters  
  - Kernel size 3 × 3  

- Max Pooling Layer

- Flatten Layer  
  Converts feature maps into a vector.

- Dense Layer  
  - 64 neurons  
  - ReLU activation

- Dropout Layer  
  - 0.5 dropout rate  
  - Prevents overfitting

- Output Layer  
  - 10 neurons  
  - Softmax activation

## Training Configuration

- Optimizer. Adam
- Loss Function. Categorical Crossentropy
- Batch Size. 32
- Epochs. 20
- Metrics. Accuracy

## Project Workflow

1 Load CIFAR-10 dataset  
2 Normalize pixel values between 0 and 1  
3 Convert labels to one hot encoding  
4 Build CNN model  
5 Train model using training dataset  
6 Validate using test dataset  
7 Evaluate final model accuracy  
8 Plot training accuracy and loss graphs  
9 Visualize sample images with labels

## Installation

Install required libraries

```bash
pip install tensorflow matplotlib pandas numpy
