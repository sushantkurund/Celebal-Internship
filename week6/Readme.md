<div align="center">

# Week 6 - Convolutional Denoising Autoencoder using MNIST

### Celebal Technologies Summer Internship 2026

Build and train a Convolutional Denoising Autoencoder (CDAE) to reconstruct clean handwritten digit images from noisy inputs using the MNIST dataset.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?logo=keras)
![Status](https://img.shields.io/badge/Status-Completed-success)

</div>

---

# Project Overview

This project implements a Convolutional Denoising Autoencoder using TensorFlow and Keras to remove Gaussian noise from handwritten digit images. The model learns meaningful image representations and reconstructs clean images from noisy inputs, demonstrating the effectiveness of encoder-decoder architectures for image restoration tasks.

---

# Objectives

- Load and preprocess the MNIST PNG dataset.
- Add Gaussian noise to the input images.
- Build a Convolutional Denoising Autoencoder.
- Train the model using noisy images as input and clean images as targets.
- Evaluate reconstruction quality using Mean Squared Error (MSE).
- Visualize the denoising performance.

---

# Dataset

This project uses the **MNIST PNG Dataset**.

> **Note:** The dataset is not included in this repository.

Place the provided `archive.zip` file in the project directory before running the notebook.

After extraction, the folder structure should be:

```text
mnist_png/
├── training/
└── testing/
```

---

# Tech Stack

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pillow (PIL)
- Scikit-learn

---

# Model Architecture

```
Input Image (28×28×1)
        │
Conv2D (32)
        │
MaxPooling2D
        │
Conv2D (64)
        │
MaxPooling2D
        │
 Bottleneck
        │
UpSampling2D
        │
Conv2D (64)
        │
UpSampling2D
        │
Conv2D (32)
        │
Conv2D (1)
        │
Denoised Image
```

---

# Model Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Mean Squared Error (MSE) |
| Epochs | 20 |
| Batch Size | 128 |
| Validation Split | 10% |
| Callback | Early Stopping |

---

# Results

## Sample Original Images

The following images are sample handwritten digits from the MNIST dataset before any preprocessing or noise is added.

<p align="center">
<img src="assets/original_images.png" width="750">
</p>

---

## Original vs Noisy Images

Gaussian noise is added to the original images to create the training input for the autoencoder.

<p align="center">
<img src="assets/original_noisy.png" width="750">
</p>

---

## Original vs Noisy vs Denoised Images

After training, the model successfully reconstructs clean images by removing most of the added noise while preserving the important features of each handwritten digit.

<p align="center">
<img src="assets/denoised_results.png" width="750">
</p>

---

## Training and Validation Loss

The training and validation loss decrease consistently during training, showing that the model learns effective image representations while maintaining good generalization.

<p align="center">
<img src="assets/training_loss.png" width="750">
</p>

---

# Results Summary

- Successfully implemented a Convolutional Denoising Autoencoder.
- Added Gaussian noise to MNIST images for supervised denoising.
- Reconstructed clean images with good visual quality.
- Achieved consistent reduction in training and validation loss.
- Evaluated reconstruction performance using Mean Squared Error (MSE).

---

# Repository Structure

```text
week6/
│── assets/
│   ├── original_images.png
│   ├── original_noisy.png
│   ├── denoised_results.png
│   └── training_loss.png
│
├── Week6_Sushant_DPGU.ipynb
└── README.md
```

---

# How to Run

1. Clone this repository.
2. Place `archive.zip` inside the project directory.
3. Open the notebook using Google Colab or Jupyter Notebook.
4. Run all cells sequentially.

---

# Author

**Sushant Kurund**

MCA (Data Science)

Celebal Technologies Summer Internship 2026
