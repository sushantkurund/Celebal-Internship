# CIFAR-10 Image Classification using Artificial Neural Networks and Convolutional Neural Networks

## Introduction

This project was completed as part of **Week 4** of the **Celebal Technologies Data Science Internship**. The goal was to explore deep learning techniques for image classification by implementing both an **Artificial Neural Network (ANN)** and a **Convolutional Neural Network (CNN)** on the CIFAR-10 dataset. In addition to building baseline models, the project investigates the effect of model improvements such as data augmentation, deeper architectures, and EarlyStopping.

---

## About the Dataset

The models were trained and evaluated using the **CIFAR-10** benchmark dataset, which is widely used for image classification tasks.

**Dataset Details**

- Total Images: 60,000
- Training Images: 50,000
- Testing Images: 10,000
- Image Resolution: 32 × 32 pixels
- Color Format: RGB
- Number of Categories: 10

### Image Categories

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

## Project Pipeline

The implementation follows a complete deep learning workflow:

- Load and inspect the CIFAR-10 dataset
- Normalize image pixel values
- Prepare image data for ANN and CNN architectures
- Train a baseline ANN model
- Train a baseline CNN model
- Compare model performance
- Improve the CNN using advanced training techniques
- Evaluate and analyze the final results

---

## Data Preparation

Before training, the following preprocessing steps were applied:

- Pixel values were scaled from **0–255** to **0–1**
- Images were flattened into one-dimensional vectors for the ANN
- Original image dimensions were retained for the CNN
- Sample images were visualized to verify the dataset

---

## Model Architectures

### Artificial Neural Network (ANN)

The ANN serves as a baseline model for comparison.

Architecture includes:

- Flatten Layer
- Dense Layers
- Dropout Regularization
- Softmax Output Layer

This model learns from flattened image vectors without preserving spatial relationships between pixels.

---

### Convolutional Neural Network (CNN)

The CNN is designed specifically for image data.

Layers used include:

- Conv2D
- BatchNormalization
- MaxPooling2D
- Flatten
- Dense
- Dropout
- Softmax Output

Unlike the ANN, the CNN extracts meaningful spatial features directly from the images.

---

## Model Training

Both models were trained using the following configuration:

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Evaluation Metric | Accuracy |
| Batch Size | 64 |
| Validation Split | 10% |

The baseline models were trained for **10 epochs**, while the enhanced CNN was trained for **20 epochs** with EarlyStopping enabled.

---

## Performance Improvements

Several enhancements were introduced to improve the CNN model:

- Increased the number of Dense layers in the ANN
- Expanded convolutional filters from **32 → 64 → 128**
- Increased training duration to **20 epochs**
- Applied **EarlyStopping** to reduce overfitting
- Introduced image augmentation using:
  - RandomFlip
  - RandomRotation
  - RandomZoom

These modifications were implemented to improve learning efficiency and model generalization.

---

## Model Comparison

| Model | Description |
|--------|-------------|
| ANN | Baseline fully connected neural network trained on flattened images |
| CNN | Convolution-based architecture capable of learning spatial image features |
| Enhanced CNN | CNN with data augmentation, deeper architecture, and EarlyStopping |

---

## Technologies and Libraries

The project was implemented using:

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Google Colab

---

## Key Findings

The experimental results highlight several important observations:

- CNN consistently achieved higher classification accuracy than the ANN.
- Preserving spatial information significantly improves image recognition performance.
- Data augmentation increased the model's ability to generalize to unseen images.
- EarlyStopping reduced unnecessary training and helped prevent overfitting.
- Increasing the depth of the network enabled the model to learn more complex image features.

---

## Learning Outcomes

Through this assignment, I gained practical experience in:

- Image preprocessing techniques
- Artificial Neural Networks (ANN)
- Convolutional Neural Networks (CNN)
- Feature extraction using convolution
- Batch Normalization
- Dropout Regularization
- Data Augmentation
- EarlyStopping
- Model evaluation and comparison
- Deep learning model development using TensorFlow and Keras

---

## Repository Structure

```
Week4/
├── CIFAR10_ANN_CNN_Learning_Project.ipynb
└── README.md
```

---

## Conclusion

This project demonstrates the importance of selecting an appropriate neural network architecture for image classification tasks. While the ANN provides a useful baseline, the CNN delivers significantly better performance by preserving spatial information and learning hierarchical visual features. Additional techniques such as data augmentation and EarlyStopping further enhance the robustness and accuracy of the model.

---

## Author

**Sushant**

MCA (Data Science)

Celebal Technologies – Data Science Internship
