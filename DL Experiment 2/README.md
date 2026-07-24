# Comparative Study of Activation Functions and Optimization Algorithms

**Author:** Rohith John M  
**Roll No:** 24BAD100  

## Aim
To analyze the impact of different activation functions and optimization algorithms on the performance of Artificial Neural Networks (ANNs) and to implement best practices for managing deep learning experiments.

## Software Requirements
* Python 3.x
* TensorFlow / Keras
* Scikit-learn
* Matplotlib
* NumPy
* Google Colab

## Project Overview

This repository contains the implementation of a comparative analysis divided into three distinct parts:

### Part A: Visualization of Activation Functions
* Implemented the mathematical definitions and derivatives for three fundamental activation functions: **Sigmoid**, **Tanh**, and **ReLU**.
* Generated visualization subplots to analyze the output ranges, saturation regions, and gradient behavior of each function.
* Provided a theoretical comparison regarding computational efficiency and typical applications in deep neural networks.

### Part B: Performance Comparison of Activation Functions
* Built three identical ANN architectures to classify the Breast Cancer Wisconsin dataset.
* Trained each network using a different hidden layer activation function (Sigmoid, Tanh, ReLU).
* Utilized the `EarlyStopping` callback to accurately measure the number of epochs required for convergence.
* **Key Finding:** ReLU demonstrated the fastest convergence and highest computational efficiency by mitigating the vanishing gradient problem, whereas Sigmoid required the most epochs and exhibited slower convergence.

### Part C: Comparison of Optimization Algorithms
* Trained identical ANN models (using the optimal ReLU activation) on the same dataset using four distinct gradient-based optimizers: **SGD**, **Momentum**, **RMSprop**, and **Adam**.
* Evaluated and plotted the convergence speed, training loss, and final validation accuracy for each algorithm across a fixed number of epochs.
* **Key Finding:** Adam provided the most reliable balance of high final validation accuracy and rapid, stable convergence due to its adaptive learning rate, outperforming standard SGD and Momentum.

## Execution Instructions
1. Clone this repository to your local machine or open it directly in GitHub.
2. Open the `Study_of_Activation_Functon.ipynb` notebook using Google Colab or a local Jupyter Notebook environment.
3. Ensure all dependencies are installed in your environment:
   ```bash
   pip install tensorflow scikit-learn matplotlib numpy pandas