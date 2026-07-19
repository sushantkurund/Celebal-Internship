# Week 6 Assignment – Convolutional Denoising Autoencoder using MNIST

## Overview

This project implements a **Convolutional Denoising Autoencoder (CDAE)** using TensorFlow and Keras to remove Gaussian noise from handwritten digit images in the MNIST dataset. The model is trained to reconstruct clean images from noisy inputs, demonstrating the application of deep learning in image restoration.

---

## Objective

The objective of this assignment is to:

- Load and preprocess the MNIST handwritten digit dataset.
- Add Gaussian noise to the images.
- Build a Convolutional Denoising Autoencoder.
- Train the model using noisy images as input and clean images as output.
- Evaluate the reconstruction performance using Mean Squared Error (MSE).
- Visualize the original, noisy, and reconstructed images.

---

## Dataset

- **Dataset:** MNIST PNG Dataset
- **Training Images:** 60,000
- **Testing Images:** 10,000
- **Image Size:** 28 × 28 pixels
- **Color Format:** Grayscale

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

1. Import required libraries.
2. Verify TensorFlow installation.
3. Extract the MNIST dataset.
4. Verify dataset structure.
5. Count training and testing images.
6. Load and normalize images.
7. Reshape images for CNN input.
8. Display sample images.
9. Add Gaussian noise.
10. Compare original and noisy images.
11. Build the Convolutional Denoising Autoencoder.
12. Compile the model.
13. Configure Early Stopping.
14. Train the model.
15. Plot training and validation loss.
16. Generate denoised images.
17. Compare original, noisy, and reconstructed images.
18. Evaluate reconstruction using Mean Squared Error (MSE).

---

## Model Architecture

### Encoder
- Conv2D (32 filters)
- MaxPooling2D
- Conv2D (64 filters)
- MaxPooling2D

### Bottleneck
- Conv2D (64 filters)

### Decoder
- UpSampling2D
- Conv2D (64 filters)
- UpSampling2D
- Conv2D (32 filters)
- Conv2D (1 filter, Sigmoid Activation)

---

## Model Configuration

| Parameter | Value |
|-----------|--------|
| Optimizer | Adam |
| Loss Function | Mean Squared Error (MSE) |
| Epochs | 20 |
| Batch Size | 128 |
| Validation Split | 10% |
| Callback | Early Stopping |

---

## Results

The trained Convolutional Denoising Autoencoder successfully reconstructed clean handwritten digit images from noisy inputs.

Key observations:

- Gaussian noise was effectively removed from the images.
- Training and validation loss decreased steadily.
- Early Stopping prevented unnecessary training.
- The reconstructed images preserved the important digit features.
- A low Mean Squared Error (MSE) indicated good reconstruction quality.

---

## Conclusion

This project demonstrates the effectiveness of Convolutional Denoising Autoencoders for image denoising tasks. By learning meaningful image representations, the model successfully restored noisy handwritten digit images while preserving their important structural features.

The assignment provides practical experience in image preprocessing, convolutional neural networks, autoencoders, model training, and evaluation using TensorFlow and Keras.

---

## Author

**Name:** Sushant  
**Course:** MCA (Data Science)  
**Organization:** Celebal Technologies – Summer Internship Program 2026
