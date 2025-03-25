# Fashion-MNIST-Modeling-Comparision
## Overview

This project is part of the TAMU ECEN 758 Data Mining and Analysis course. The goal is to classify articles of clothing using the FashionMNIST dataset. This study implements and compares the performance of:
- Convolutional Neural Networks (CNNs)
- LightGBM (Gradient Boosting Decision Trees)

Through this project, we gained hands-on experience with PyTorch and various ML/Data packages while deepening our understanding of the theoretical foundations of Convolutional Neural Networks (CNNs) and Gradient Boosting Decision Trees, specifically LightGBM. Additionally, it enhanced our problem-solving approach in machine learning applications.

Checkout our project post on Medium: https://medium.com/@emilyjyc/comparison-of-cnn-and-light-gbm-with-fashion-mnist-77cd1644810e

## Dataset
We use the FashionMNIST dataset, which contains:
- 60,000 training images and 10,000 test images
- 10 clothing categories (e.g., T-shirt, pants, dress, etc.)
- 28×28 grayscale images
More details: [FashionMNIST GitHub](https://github.com/zalandoresearch/fashion-mnist)

## Methodology

### 1. Data Preparation
- Normalization & Standardization
- Train/Test Split (80/20)
- Data Augmentation (for CNNs)
  
### 2. Exploratory Data Analysis (EDA)
- Class distribution visualization
- Example images from each class
- Dimensionality reduction (e.g., PCA, t-SNE)
  
### 3. Model Selection & Training

#### Model 1: Convolutional Neural Networks (CNNs)
- Implemented using PyTorch
- Uses multiple convolutional layers with batch normalization
- Optimized with Adam optimizer and cross-entropy loss
  
#### Model 2: LightGBM
- Gradient Boosting Decision Trees (GBDT) implementation
- Uses histogram-based feature learning
- Optimized with early stopping and learning rate tuning
  
### 4. Model Evaluation
- Accuracy, Precision, Recall, F1-score
- Confusion Matrix Analysis
- Feature Importance (for LightGBM)

## Basic Parameters Configuration

### Deep CNN (Pytorch)
- Criterion: CrossEntropy
- Optimizer: Adam
- Learning rate: 0.001
- Early-stopping rounds: 5

### LightGBM
- Number of leaves in full tree: 31
- Learning rate: 0.05
- Part of feature to be used for each iteration: 0.9
- Part of data to be used for each iteration: 0.8
- Early-stopping round: 5

## Conclusion
CNNs achieved 3.35% higher accuracy than LightGBM, making them ideal for image classification tasks requiring intricate pattern recognition. However, LightGBM was 730 seconds faster, making it more suitable for real-time applications like inventory updates. Future work could explore hybrid models that leverage the strengths of both approaches.
