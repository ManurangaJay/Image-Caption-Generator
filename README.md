# Automated Image Captioning System using Deep Learning

This project implements and evaluates two deep-learning models for generating captions from images. The work explores different architectures, including **VGG16 with LSTM** and **ResNet50 with a Transformer**, to enable automatic image description. It highlights the potential of AI in **image understanding** and accessibility, with applications in **content retrieval** and **human-computer interaction**.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Model Architectures](#model-architectures)
- [Performance Evaluation](#performance-evaluation)

## Overview
As part of the **Deep Learning module** at the **University of Jaffna**, this project investigates the application of deep learning in **image caption generation**. The study developed two models:
1. **VGG16 with LSTM**
2. **ResNet50 with a Transformer**

These models were trained and tested on a dataset of 8,091 images, each paired with human-generated captions. The performance was assessed using **BLEU scores**, with the **VGG16-LSTM model** achieving superior accuracy.

## Features
- **Image Preprocessing**:
  - Resizing and normalizing pixel values for deep learning models.
  - Caption tokenization for model training.
- **Model Architectures**:
  - A sequential pipeline combining **VGG16** (feature extraction) and **LSTM** (caption generation).
  - A transformer-based pipeline using **ResNet50** for feature extraction.
- **Performance Metrics**:
  - Evaluation through **BLEU scores** to measure the quality of generated captions.

## Technologies Used
- **Deep Learning Frameworks**: TensorFlow, Keras
- **Pretrained Models**: VGG16, ResNet50
- **Programming Language**: Python
- **Evaluation Metrics**: BLEU Scores
- **Development Environment**: Jupyter Notebook

## Dataset
- **Source**: The dataset comprises 8,091 images, each paired with 5 human-generated captions.
- **Preprocessing Steps**:
  - Resized images to a standard dimension.
  - Normalized pixel values to [0, 1].
  - Tokenized captions and built a vocabulary for text representation.

## Model Architectures
### 1. **VGG16 with LSTM**
- **Feature Extraction**: Uses the VGG16 model (pretrained on ImageNet) to extract features from images.
- **Caption Generation**: A Long Short-Term Memory (LSTM) network generates captions based on extracted features and tokenized input.
- **Performance**: Achieved better BLEU scores compared to ResNet50-Transformer.

### 2. **ResNet50 with Transformer**
- **Feature Extraction**: Utilizes ResNet50 (pretrained on ImageNet) to extract image features.
- **Caption Generation**: A Transformer network processes the features and generates captions.
- **Performance**: Slightly less accurate than VGG16-LSTM in this implementation.

## Performance Evaluation
The models were evaluated using **BLEU scores**, a standard metric for assessing the quality of text generation models. Results showed:
- **VGG16-LSTM**: Higher accuracy and better overall caption quality.
- **ResNet50-Transformer**: Promising performance but less consistent in generating accurate captions.
