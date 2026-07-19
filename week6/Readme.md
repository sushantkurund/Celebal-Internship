# Week 6 Assignment – Convolutional Denoising Autoencoder using MNIST

## Overview

This project implements a **Convolutional Denoising Autoencoder (CDAE)** using TensorFlow and Keras to remove Gaussian noise from handwritten digit images. The model learns to reconstruct clean images from noisy inputs using the MNIST handwritten digit dataset.

---

## Objective

The objective of this project is to:

- Load and preprocess the MNIST dataset.
- Add Gaussian noise to the images.
- Build and train a Convolutional Denoising Autoencoder.
- Reconstruct clean images from noisy inputs.
- Evaluate the model using Mean Squared Error (MSE).
- Visualize the denoising results.

---

## Dataset

This project uses the **MNIST PNG Dataset**.

**Note:** The dataset is **not included** in this repository to keep it lightweight.

Place the provided `archive.zip` file in the project directory before running the notebook.

Dataset structure after extraction:

```text
mnist_png/
├── training/
│   ├── 0/
│   ├── 1/
│   └── ...
└── testing/
    ├── 0/
    ├── 1/
    └── ...
```

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pillow (PIL)
- Scikit-learn

---

## Project Workflow

1. Import required libraries
2. Extract the dataset
3. Load and preprocess images
4. Add Gaussian noise
5. Build the Convolutional Denoising Autoencoder
6. Train the model
7. Generate denoised images
8. Evaluate using Mean Squared Error (MSE)
9. Visualize the results

---

## Model Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Mean Squared Error (MSE) |
| Epochs | 20 |
| Batch Size | 128 |
| Validation Split | 10% |
| Callback | Early Stopping |

---

## Results

The trained model successfully removed Gaussian noise from handwritten digit images.

Key observations:

- Training and validation loss decreased consistently.
- Early Stopping prevented overfitting.
- The reconstructed images closely matched the original images.
- A low Mean Squared Error (MSE) indicated good reconstruction performance.

---

## Repository Structure

```text
Week-6/
│── Week6_Sushant_DPGU.ipynb
└── README.md
```

---

## How to Run

1. Clone this repository.
2. Place `archive.zip` in the project directory.
3. Open the notebook in Google Colab or Jupyter Notebook.
4. Run all cells sequentially.

---

## Author

**Sushant**  
**MCA (Data Science)**  
**Celebal Technologies – Summer Internship Program 2026**
