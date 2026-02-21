# Vision Transformer (ViT) From Scratch — TensorFlow Implementation

This project implements a Vision Transformer (ViT) architecture completely from scratch using TensorFlow / Keras — without using any pretrained ViT model.

The goal of this project is to understand how transformers work on images internally rather than using ready-made architectures.
__________________________________________________________________________________________________________________________________

📌 Project Objective

To build a deep learning image classifier using the Transformer architecture instead of CNNs by:

Converting images into patches

Encoding positional information

Passing them through multi-head self-attention layers

Learning global relationships between pixels

This project focuses on learning the architecture — not just achieving accuracy.
__________________________________________________________________________________________________________________________________

🧠 What is Vision Transformer?

Traditional CNNs detect local patterns (edges → textures → objects).

Vision Transformers instead:

Split image into small patches

Treat patches like words in NLP

Use self-attention to understand relationships across the entire image

So the model learns global context directly instead of gradually expanding receptive field.

__________________________________________________________________________________________________________________________________

What the Model Does

The model performs image classification by:

Splitting images into fixed-size patches (16×16)

Converting patches into embeddings

Adding positional encoding

Passing them through stacked Transformer encoder layers

Classifying the image using an MLP head

Image → Patches → Embedding → Transformer Layers → MLP → Softmax
Key Components Implemented

Patch extraction using tf.image.extract_patches

Positional embeddings

Multi-Head Self-Attention

Residual connections

Transformer encoder blocks

Classification head

No pretrained ViT weights were used.

__________________________________________________________________________________________________________________________________

Purpose

This project focuses on learning the internal working of Vision Transformers and understanding how global relationships in images can be captured using attention instead of convolution.

Dataset

The dataset is downloaded automatically via Kaggle API inside the notebook (not stored in the repo).

How to Run

Install requirements

Download dataset from notebook cell

Train and evaluate the model
__________________________________________________________________________________________________________________________________

Educational implementation — focused on architecture understanding rather than performance optimization.