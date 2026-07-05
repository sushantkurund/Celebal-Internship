# CIFAR-10 Image Classification using ANN and CNN

## Overview

This project implements and compares image classification models using an Artificial Neural Network (ANN) and a Convolutional Neural Network (CNN) on the CIFAR-10 dataset. It demonstrates the advantages of CNNs for image-based tasks and explores training improvements such as data augmentation and Early Stopping.

---

## Problem Statement

Build an image classification model on the CIFAR-10 dataset and analyze the performance of different neural network architectures and training strategies.

The project includes:

- Baseline Artificial Neural Network (ANN)
- Convolutional Neural Network (CNN)
- Performance comparison
- Validation accuracy visualization
- Data augmentation
- EarlyStopping
- Model performance analysis

---

## Dataset

**Dataset:** CIFAR-10

The dataset contains **60,000 RGB images** of size **32 × 32** belonging to **10 classes**.

- Training Images: 50,000
- Test Images: 10,000

### Classes

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

---

## Project Workflow

1. Load the CIFAR-10 dataset
2. Visualize sample images
3. Normalize image pixel values
4. Flatten images for the ANN model
5. Build and train the ANN
6. Build and train the CNN
7. Compare ANN and CNN performance
8. Plot validation accuracy curves
9. Apply data augmentation
10. Train an improved CNN with EarlyStopping
11. Evaluate model performance

---

## Models Implemented

### 1. Artificial Neural Network (ANN)

Architecture

- Flatten
- Dense (512)
- Dropout
- Dense (256)
- Dropout
- Dense (128)
- Dense (64)
- Output Layer (Softmax)

---

### 2. Convolutional Neural Network (CNN)

Architecture

- Conv2D (32)
- BatchNormalization
- MaxPooling2D
- Conv2D (64)
- BatchNormalization
- MaxPooling2D
- Conv2D (128)
- BatchNormalization
- MaxPooling2D
- Flatten
- Dense
- Dropout
- Output Layer

---

### 3. Augmented CNN

Additional preprocessing layers:

- RandomFlip
- RandomRotation
- RandomZoom

Training improvements:

- EarlyStopping
- 20 Epochs

---

## Training Configuration

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Metric: Accuracy
- Batch Size: 64
- Validation Split: 10%
- Epochs:
  - Baseline Models: 10
  - Improved Model: 20

---

## Student Learning Tasks Completed

- Increased ANN architecture
- Increased CNN filters (32 → 64 → 128)
- Increased training epochs to 20
- Added EarlyStopping
- Implemented Data Augmentation
- Compared ANN and CNN performance

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab

---

## Results

The CNN significantly outperformed the ANN because convolutional layers preserve spatial information and automatically learn hierarchical image features. Data augmentation and EarlyStopping further improved model generalization and reduced overfitting.

---

## Conclusion

This project demonstrates that:

- ANNs can perform image classification but are limited because they flatten image data and lose spatial relationships.
- CNNs achieve much higher accuracy by learning local and hierarchical visual features.
- Data augmentation improves model robustness.
- EarlyStopping helps prevent overfitting and restores the best-performing model.

Overall, the enhanced CNN provided the best classification performance on the CIFAR-10 dataset.

---

## Author

**Sushant**

MCA – Data Science
Celebal Technologies Internship – Week 4
