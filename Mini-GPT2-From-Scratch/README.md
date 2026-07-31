# GPT-2 From Scratch

This project is part of the **Celebal Technologies Internship – Week 8** and demonstrates the implementation of a **GPT-2 inspired Decoder-Only Transformer** built entirely from scratch using **PyTorch**. The model is trained on the **Tiny Shakespeare** dataset, served through a **FastAPI** backend, and accessed through a **React + Vite** frontend.

---

# Project Overview

This project demonstrates the complete implementation of a miniature GPT-2 style language model without relying on high-level transformer libraries.

The primary objective is to gain a practical understanding of Transformer-based language models by manually implementing each major component, including:

- Character-Level Tokenization
- Embedding Layers
- Positional Embeddings
- Multi-Head Self-Attention
- Transformer Decoder Blocks
- Autoregressive Text Generation
- Model Training
- Model Inference

The trained model generates Shakespeare-style text from user-provided prompts through an interactive web application.

---

# Features

- Character-Level Tokenizer
- GPT-2 Inspired Decoder-Only Transformer
- Multi-Head Self-Attention
- Positional Embeddings
- Transformer Decoder Blocks
- Temperature-Based Sampling
- Character-Level Text Generation
- Automatic Model Checkpoint Saving
- FastAPI REST API
- React + Vite Frontend
- Adjustable Temperature
- Adjustable Maximum Tokens
- Copy Generated Text
- Download Generated Text
- Responsive User Interface

---

# Project Architecture

```text
                  Tiny Shakespeare Dataset
                            │
                            ▼
                   Character Tokenizer
                            │
                            ▼
                 Character Embedding Layer
                            │
                            ▼
                Positional Embedding Layer
                            │
                            ▼
        Decoder-Only Transformer (GPT Style)
                            │
                            ▼
              Multi-Head Self Attention
                            │
                            ▼
                   Feed Forward Network
                            │
                            ▼
                     Language Model Head
                            │
                            ▼
                 Next Character Prediction
                            │
                            ▼
                     Generated Text Output
```

---

# Project Structure

```text
Week-8-Mini-GPT2-From-Scratch/

├── assets/
│   ├── home-page.png
│   ├── generated-output.png
│   └── swagger-ui.png
│
├── backend/
│   └── main.py
│
├── checkpoints/
│   └── model.pth
│
├── data/
│   └── tinyshakespeare.txt
│
├── frontend/
│   ├── public/
│   ├── src/
│   ├── package.json
│   ├── package-lock.json
│   ├── vite.config.js
│   └── index.html
│
├── notebook/
│   └── MiniGPT2.ipynb
│
├── outputs/
│   └── sample_output.txt
│
├── src/
│   ├── __init__.py
│   ├── attention.py
│   ├── dataset.py
│   ├── generate.py
│   ├── model.py
│   ├── tokenizer.py
│   ├── train.py
│   └── transformer.py
│
├── .gitignore
├── README.md
├── requirements.txt
├── test_dataset.py
└── test_tokenizer.py
```

---

# Technologies Used

| Category | Technology |
|-----------|------------|
| Programming Language | Python |
| Deep Learning Framework | PyTorch |
| Backend | FastAPI |
| Frontend | React |
| Build Tool | Vite |
| API Communication | Axios |
| Styling | CSS |
| Dataset | Tiny Shakespeare |

---

# Model Configuration

| Property | Value |
|----------|-------|
| Model Type | GPT-2 Inspired Decoder-Only Transformer |
| Tokenization | Character-Level |
| Dataset | Tiny Shakespeare |
| Context Length | 128 |
| Embedding Dimension | 128 |
| Attention Heads | 4 |
| Transformer Layers | 4 |
| Dropout | 0.2 |
| Optimizer | AdamW |
| Best Validation Loss | 1.6918 |

---

# Application Preview

## Home Page

![Home Page](assets/home-page.png)

---

## Generated Output

![Generated Output](assets/generated-output.png)

---

## Swagger API Documentation

![Swagger UI](assets/swagger-ui.png)

---

# Getting Started

This project is located inside the **Celebal Technologies Internship** repository.

Navigate to the project directory:

```bash
cd Week-8-Mini-GPT2-From-Scratch
```

---

## Create a Virtual Environment

### Windows

```bash
python -m venv env
env\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv env
source env/bin/activate
```

---

## Install Dependencies

Install the Python dependencies:

```bash
pip install -r requirements.txt
```

Install the React dependencies:

```bash
cd frontend
npm install
```
---

# Model Training

Train the model using:

```bash
python -m src.train
```

During training, the model:

- Loads the Tiny Shakespeare dataset
- Performs character-level tokenization
- Trains the decoder-only Transformer architecture
- Evaluates validation loss during training
- Saves the best-performing model checkpoint

The trained model is automatically saved to:

```text
checkpoints/model.pth
```

---

# Generate Text from Terminal

Generate text directly from the terminal:

```bash
python -m src.generate
```

Example prompt:

```text
KING
```

Example generated output:

```text
KING EDWARD IV:
Roman the shall law and his shall we, thou house;
And many we deservilure the maniston all the praying...
```

---

# Running the Backend

Navigate to the project directory:

```bash
cd Week-8-Mini-GPT2-From-Scratch
```

Start the FastAPI server:

```bash
uvicorn backend.main:app --reload
```

The backend will be available at:

```
http://127.0.0.1:8000
```

Interactive API documentation (Swagger UI):

```
http://127.0.0.1:8000/docs
```

---

# Running the Frontend

Navigate to the frontend directory:

```bash
cd frontend
```

Install the required packages:

```bash
npm install
```

Run the React development server:

```bash
npm run dev
```

Open the application in your browser:

```
http://localhost:5173
```

---

# Web Application Features

The web interface allows users to:

- Enter custom prompts
- Adjust Temperature
- Adjust Maximum Tokens
- Generate Shakespeare-style text
- Copy generated output
- Download generated output
- Clear previous output

---

# Sample Outputs

Example generated outputs are available in:

```text
outputs/
```

These demonstrate the text generation capability of the trained language model.

---

# Notebook

The complete implementation notebook is available in:

```text
notebook/
```

The notebook contains the complete experimentation, model development, and training workflow used while building the GPT-2 inspired language model.

---

# Learning Outcomes

This project provided hands-on experience with:

- Character-Level Tokenization
- Embedding Layers
- Positional Embeddings
- Self-Attention Mechanism
- Multi-Head Self-Attention
- Transformer Decoder Architecture
- Autoregressive Language Modeling
- Temperature-Based Sampling
- Model Training using PyTorch
- FastAPI Backend Development
- REST API Integration
- React Frontend Development

---

# Future Improvements

Possible enhancements include:

- Top-k Sampling
- Top-p (Nucleus) Sampling
- Beam Search Decoding
- Learning Rate Scheduling
- Mixed Precision Training
- Multilingual Dataset Training
- Word-Level or Subword Tokenization
- Larger GPT Configurations
- GPU Optimized Training
- Docker Deployment

---

# References

- Andrej Karpathy – Neural Networks: Zero to Hero
- PyTorch Documentation
- FastAPI Documentation
- React Documentation
- Tiny Shakespeare Dataset

---

# Author

**Sushant Kurund**

Master of Computer Applications (Data Science)

GitHub Profile:

https://github.com/sushantkurund

---

# Acknowledgements

This project was developed as part of the **Celebal Technologies Internship – Week 8**. It is inspired by the educational work of Andrej Karpathy on implementing GPT-style language models from scratch.

---

# License

This project is intended for educational purposes and demonstrates the implementation of a miniature GPT-2 inspired decoder-only Transformer architecture built entirely from scratch using PyTorch.
