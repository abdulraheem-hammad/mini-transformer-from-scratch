# Mini Transformer from Scratch with BPE Tokenizer

This project implements a minimal Transformer-based language model **alongside a Byte Pair Encoding (BPE) tokenizer built entirely from scratch in Python**. It is designed to help deeply understand the core building blocks of modern language models, including tokenization and the Transformer architecture.

 **Note:** This is an educational project. The model and tokenizer are intentionally simple and serve as a learning tool rather than a production-ready system.

---

## Project Overview

The project consists of two main components:

### 1. From-Scratch BPE Tokenizer
- Implements Byte Pair Encoding (BPE) tokenization without relying on external libraries.
- Learns merge operations from a sample corpus (`input.txt`).
- Supports training, encoding, decoding, saving, and loading.
- Produces a custom vocabulary tailored to the training text.

### 2. Transformer Language Model
- Implements a Transformer architecture with multi-head self-attention and feedforward layers.
- Uses the custom tokenizer's vocabulary size as input dimension.
- Trains on tokenized data from `input.txt`.


---

## Key Features

- **Custom BPE Tokenizer:**  
  Learns merges from raw UTF-8 text and creates tokens by combining frequent byte pairs, allowing efficient subword tokenization.

- **Transformer Architecture:**  
  Includes token and positional embeddings, multi-head self-attention, layer normalization, residual connections, and feedforward networks.

- **Training Pipeline:**  
  Reads raw text data, trains or loads the tokenizer, tokenizes the dataset, splits it into training and validation sets, trains the model, and periodically evaluates performance.

- **Text Generation:**  
  Generates new text  based on the learned language model.

---

**Inspiration**
This project was inspired by Andrej Karpathy’s "Let's Build GPT from Scratch".
