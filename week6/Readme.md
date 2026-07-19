<div align="center">

# Week 6 - Convolutional Denoising Autoencoder using MNIST

### Celebal Technologies Summer Internship 2026

Build and train a Convolutional Denoising Autoencoder (CDAE) to reconstruct clean handwritten digit images from noisy inputs using the MNIST dataset.

<img src="assets/cover.png" width="850">

<br>

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?logo=keras)
![Status](https://img.shields.io/badge/Status-Completed-success)

</div>

---

# Project Overview

This project demonstrates the implementation of a Convolutional Denoising Autoencoder using TensorFlow and Keras.

The model learns to remove Gaussian noise from handwritten digit images and reconstruct clean images while preserving important visual features.

---

# Objectives

- Load and preprocess the MNIST PNG dataset.
- Add Gaussian noise to the input images.
- Build a Convolutional Denoising Autoencoder.
- Train the model to reconstruct clean images.
- Evaluate reconstruction quality using Mean Squared Error (MSE).
- Compare the original, noisy, and reconstructed images.

---

# Dataset

This project uses the **MNIST PNG Dataset**.

> **Note:** The dataset is **not included** in this repository.

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

## Training and Validation Loss

The training and validation loss decrease steadily throughout training, showing that the model successfully learns to reconstruct clean images without significant overfitting.

<p align="center">
<img src="assets/training_loss.png" width="750">
</p>

---

## Original and Noisy Images

Gaussian noise is added to the original MNIST images before they are passed to the autoencoder.

<p align="center">
<img src="assets/original_noisy.png" width="750">
</p>

---

## Image Reconstruction

The trained autoencoder removes most of the noise while preserving the important features of each handwritten digit.

<p align="center">
<img src="assets/denoised_results.png" width="750">
</p>

---

# Repository Structure

```text
week6/
│── assets/
│   ├── cover.png
│   ├── training_loss.png
│   ├── original_noisy.png
│   └── denoised_results.png
│
│── Week6_Sushant_DPGU.ipynb
└── README.md
```

---

# How to Run

1. Clone the repository.
2. Place `archive.zip` in the project directory.
3. Open the notebook in Google Colab or Jupyter Notebook.
4. Run all the cells sequentially.

---

# Author

**Sushant Kurund**

MCA (Data Science)

Celebal Technologies Summer Internship 2026
