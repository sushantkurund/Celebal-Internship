# Week 5 – Text Generation using RNN, LSTM, and GRU

## Overview

This project demonstrates text generation using three different recurrent neural network architectures: **Simple RNN**, **LSTM**, and **GRU**. The notebook follows a complete deep learning workflow, including text preprocessing, sequence generation, model training, performance comparison, and next-word prediction.

In addition to the base implementation, the required student customization tasks have been completed to enhance the models and compare their performance.

---

## Objectives

- Preprocess and tokenize a text corpus.
- Create n-gram sequences for next-word prediction.
- Build and train Simple RNN, LSTM, and GRU models.
- Compare model training performance using loss curves.
- Generate text from a common seed phrase.
- Complete the required student customization tasks.

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib

---

## Project Workflow

1. Load and preprocess the text corpus.
2. Convert words into integer tokens using the Keras Tokenizer.
3. Generate n-gram sequences and apply sequence padding.
4. Split the data into input features and target labels.
5. Build three deep learning models:
   - Simple RNN
   - LSTM
   - GRU
6. Train each model using the Adam optimizer.
7. Compare training loss across all models.
8. Generate text using a common seed phrase.

---

## Student Learning Task Customizations

The following customization tasks were completed as part of the assignment:

- Replaced the default boilerplate text with a custom AI-related paragraph.
- Increased the embedding dimension from **32** to **128**.
- Increased hidden layer size from **64** to **128**.
- Extended model training from **100** to **200** epochs.
- Modified the text generation output from **5** words to **10** words.

---

## Models Implemented

### Simple RNN
A basic recurrent neural network used for sequence learning and next-word prediction.

### LSTM
An advanced recurrent network capable of learning long-term dependencies using memory cells and gating mechanisms.

### GRU
A simplified recurrent architecture that provides performance similar to LSTM while using fewer parameters.

---

## Evaluation

The notebook includes:

- Training loss comparison of RNN, LSTM, and GRU models.
- Text generation using the same seed phrase for all three models.
- Enhanced models trained with the required customization tasks.

---

## Learning Outcomes

After completing this project, I gained practical experience in:

- Text preprocessing for Natural Language Processing (NLP)
- Word tokenization and sequence generation
- Building recurrent neural network architectures
- Comparing RNN, LSTM, and GRU performance
- Next-word prediction and text generation
- Improving model performance through architectural modifications

---

## Author

**Sushant Kurund**

MCA – Data Science  
Dnyaan Prasad Global University (DPGU)

Week 5 Assignment – Deep Learning (Text Generation using RNN, LSTM, and GRU)
