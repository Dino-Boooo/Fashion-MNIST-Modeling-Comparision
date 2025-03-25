# Fashion-MNIST-Modeling-Comparision
This project is focused on comparing two distinct models, the Deep Convolutional Neural Networks (CNNs) and the Light Gradient Boosting Machine (LightGBM), to determine their effectiveness in image classification using the FashionMNIST dataset.

By working through this project, we have a chance to work on Pytorch and ML/Data packages, also we can dive deeper into the theoretical foundations of CNNs and Gradient Boosting Decision Tree (specifically LightGBM) and the problem-solving thoughts.

Checkout our project post on Medium: https://medium.com/@emilyjyc/comparison-of-cnn-and-light-gbm-with-fashion-mnist-77cd1644810e

## Basic Parameters Configuration

### Deep CNN (Pytorch)
Criterion: CrossEntropy
Optimizer: Adam
Learning rate: 0.001
Early-stopping rounds: 5

### LightGBM
Number of leaves in full tree: 31
Learning rate: 0.05
Part of feature to be used for each iteration: 0.9
Part of data to be used for each iteration: 0.8
Early-stopping round: 5

## Future Work
Use hyperparameter tunning techniques such as GridSearch or RandomSearch.
