---
title: Deep Learning Image Classification Model
publishDate: 2025-04-03 00:00:00
img: /assets/neuralnet.jpg
img_alt: Blue Background with a human face wire connected   to a R logo.
description: |
  Developed an image classification pipeline leveraging pre-trained ResNet-18 and ResNet-34 architectures within PyTorch, fine-tuned for a custom multi-class dataset. The project encompasses data preprocessing, model training, evaluation, and visualization of results.
tags:
  - Deep Learning
  - Convolutional Neural Networks
  - Image Classification
  - Pytorch
  - Resnet 16 and 34
  - Data Augumentation
---

This project focuses on classifying images into multiple categories using deep learning techniques. Utilizing PyTorch and its torchvision library, the workflow involves loading and preprocessing image data, fine-tuning pre-trained ResNet models, and evaluating their performance on a custom dataset.

**Data Preprocessing**

The dataset comprises images categorized into distinct classes. Images are loaded using PyTorch's ImageFolder utility, which organizes data based on directory structure. Standard transformations, including resizing, normalization, and data augmentation techniques like random horizontal flips and rotations, are applied to enhance model generalization.

**Model Architecture and Training**

Pre-trained ResNet-18 and ResNet-34 models, known for their deep residual learning capabilities, are employed. The final fully connected layers are modified to match the number of classes in the custom dataset. The models are trained using the Adam optimizer and cross-entropy loss function. Training involves forward propagation to compute predictions, loss calculation, backpropagation to compute gradients, and optimizer steps to update model weights.

**Model Evaluation and Visualization**

Model performance is assessed using accuracy metrics on validation and test datasets. Training and validation loss and accuracy are tracked across epochs to monitor learning progress and detect potential overfitting. Confusion matrices are generated to visualize classification performance across different classes.

This project demonstrates the application of transfer learning using deep convolutional neural networks for image classification tasks. By fine-tuning pre-trained models on a specific dataset, it achieves efficient and accurate classification performance.

🔗 GitHub Repository: [Image Classification Neural Network Model](https://github.com/i-archanasenthil/image-classification-model)
