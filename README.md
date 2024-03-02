# Circle Dataset Classification using PyTorch

This project demonstrates how to classify a circular dataset using PyTorch. It includes two models: a simple linear model and a more complex model with a hidden layer. The models are trained using the BCEWithLogitsLoss loss function and the SGD optimizer.

## Getting Started

### Prerequisites

- Python (>=3.6)
- PyTorch (>=1.9.0)
- scikit-learn
- matplotlib
- Jupyter Notebook

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/circle-dataset-classification.git
   ```

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open and run the `main.ipynb` notebook to train and evaluate the models.

## Project Structure

- `main.ipynb`: Jupyter Notebook for training and evaluating the models.
- `helper_functions.py`: Helper functions for plotting predictions and decision boundaries.
- `requirements.txt`: List of required packages.

---

# Circle Dataset Classification using PyTorch - Binary Classification

## Overview
This project demonstrates the classification of a circular dataset using PyTorch, a popular deep learning library. The goal is to build and compare two neural network models: a simple linear model and a more complex model with a hidden layer. The models are trained to classify the dataset into two classes: inner and outer circles.

## Dataset
The dataset is generated using scikit-learn's `make_circles` function, creating a circular pattern with some added noise. Each data point has two features (x and y coordinates) and a binary label indicating whether it belongs to the inner circle (class 0) or the outer circle (class 1).

## Models
1. **Linear Model (Model V0)**: This model consists of a single linear layer without any activation functions. It serves as a baseline to compare the performance of the more complex model.
2. **Neural Network with Hidden Layer (Model V1)**: This model includes a hidden layer with ReLU activation functions. The additional layer allows the model to learn more complex patterns in the dataset.

## Training and Evaluation
Both models are trained using the Binary Cross Entropy with Logits Loss (BCEWithLogitsLoss) and the Stochastic Gradient Descent (SGD) optimizer. The training process involves iterating over the dataset for a specified number of epochs, computing the loss, and updating the model parameters using backpropagation.

The trained models are evaluated on a separate test dataset to measure their accuracy in classifying the circular patterns. The accuracy metric is used to compare the performance of the models.

## Results
- **Linear Model (Model V0)**: The linear model struggles to classify the circular dataset accurately. It is unable to separate the inner and outer circles effectively, resulting in poor performance.
- **Neural Network with Hidden Layer (Model V1)**: The model with a hidden layer performs significantly better, accurately classifying the circular dataset. The additional layer allows the model to learn complex patterns, improving its ability to separate the inner and outer circles.

## Conclusion
This project demonstrates the importance of model complexity in solving classification problems with complex patterns. The addition of a hidden layer significantly improves the model's performance, highlighting the effectiveness of neural networks in handling non-linear datasets.
