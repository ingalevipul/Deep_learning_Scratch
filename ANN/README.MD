

# ANN From Scratch - MNIST Digit Classification

This project implements an Artificial Neural Network (ANN) from scratch in Python for classifying handwritten digit images from the MNIST dataset. The implementation covers all fundamental components of a fully connected neural network, including forward propagation, backpropagation, loss computation, and training with mini-batch gradient descent.

***

## Features

- Load and preprocess MNIST training and test datasets.
- Implement an ANN with one hidden layer using ReLU activation.
- Use softmax activation for the output layer to handle multi-class classification.
- Compute cross-entropy loss for training.
- Train the model using mini-batch stochastic gradient descent.
- Evaluate model accuracy on the test set.
- Compare performance with different hidden layer sizes (10 neurons vs 64 neurons).
- Visualize sample test images with predicted and actual digit labels.

***

## Files and Dependencies

- `ANN_FROM_SCRATCH.ipynb`: Jupyter notebook containing full implementation, training, testing, and visualization code.
- Requires Python packages:
    - `pandas`
    - `numpy`
    - `matplotlib`

***

## Dataset

- MNIST handwritten digits dataset.
- Training data in `mnist_train.csv` (first column as label, remaining columns as pixels).
- Test data in `mnist_test.csv` (same format as train).
- Pixel values are normalized to  before training.[^1]

***

## Usage

1. Load training and test data from CSV files.
2. Initialize ANN model specifying input dimension (784 pixels), hidden layer dimension, and output dimension (10 classes).
3. Train the model for a specified number of epochs with mini-batch updates.
4. Evaluate and print test accuracy.
5. Visualize individual test samples with predictions.

***

## Model Details

- Input layer: 784 neurons (28x28 flattened image).
- Hidden layer: configurable size (e.g., 10 or 64 neurons) with ReLU activation.
- Output layer: 10 neurons with softmax activation.
- Loss function: cross-entropy.
- Optimizer: mini-batch gradient descent with learning rate control.

***

## Results

- The notebook reports training loss and accuracy per epoch.
- Test accuracies for different hidden layer sizes are printed.
- Sample test images are displayed with predicted and actual labels.

***

## How to Run

1. Place `mnist_train.csv` and `mnist_test.csv` in the specified path or update file paths accordingly.
2. Open and run all cells in the notebook `ANN_FROM_SCRATCH.ipynb`.
3. Modify model parameters (hidden layer size, epochs, batch size, learning rate) as needed.

***

## Notes

- This implementation is intended for educational purposes to demonstrate working of ANN from the ground up without high-level deep learning libraries.
- Performance can be improved by tuning hyperparameters or adding more layers.

***

## Author

An educational project developed for practicing neural network fundamentals and digit classification by Vipul Ingale

<div style="text-align: center">⁂</div>

[^1]: ANN_FROM_SCRATCH.ipynb

