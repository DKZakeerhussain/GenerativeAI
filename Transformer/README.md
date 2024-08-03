# Transformer Implementation

This repository contains an end-to-end implementation of the Transformer model, as introduced by Vaswani et al. in their groundbreaking paper ["Attention is All You Need"](https://arxiv.org/abs/1706.03762).

## Table of Contents
- [Introduction](#introduction)
- [Architecture Overview](#architecture-overview)
- [References](#references)

## Introduction

The Transformer model has revolutionized natural language processing (NLP) and has become the foundation for many state-of-the-art models such as BERT, GPT, and T5. This repository provides an end-to-end implementation of the original Transformer model, including detailed explanations and code.

## Transformer Architecture Overview

The Transformer architecture is composed of an encoder and a decoder, each with multiple layers. The key innovation of the Transformer is the self-attention mechanism, which enables the model to weigh the importance of different words in a sequence.

### Encoder

The encoder is responsible for processing the input sequence and consists of multiple layers, each containing:

1. **Multi-Head Self-Attention**: Allows the model to attend to different parts of the input sequence simultaneously.
2. **Feed-Forward Network**: Applies a fully connected feed-forward network to each position independently.
3. **Layer Normalization and Residual Connections**: Improve training and convergence.

### Decoder

The decoder generates the output sequence and also consists of multiple layers, each containing:

1. **Masked Multi-Head Self-Attention**: Ensures that predictions for a given position depend only on the known outputs at earlier positions.
2. **Multi-Head Attention over Encoder's Output**: Allows the decoder to attend to the entire input sequence.
3. **Feed-Forward Network**: Similar to the encoder.
4. **Layer Normalization and Residual Connections**: Improve training and convergence.

## Key Components

### Multi-Head Self-Attention

The self-attention mechanism computes a representation of the input sequence by considering the importance of each word relative to others. Multi-head attention allows the model to focus on different parts of the sequence simultaneously.

### Positional Encoding

Since the Transformer does not inherently understand the order of the input sequence, positional encoding is added to the input embeddings to provide information about the position of each word.

### Feed-Forward Network

A fully connected feed-forward network is applied independently to each position in the sequence. This network typically consists of two linear transformations with a ReLU activation in between.

### Layer Normalization and Residual Connections

Layer normalization is applied to stabilize and accelerate training. Residual connections help in training deep networks by allowing gradients to flow through the network more easily.


![image](https://github.com/user-attachments/assets/1ebf0078-7885-4c7e-99ed-ddf39a70ff57)


## Refrences
- Paper ["Attention is All You Need"](https://arxiv.org/abs/1706.03762).


