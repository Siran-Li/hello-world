# Image Classification Multilayer Perceptron Network
Classifying images from the CIFAR-10 dataset using a multilayer perceptron (MLP) neural network


### Steps

The steps included:
* **Normalizing** data and **one-hot encoding** labels
* flatting the `input` data to a long feature vector
* Building a MLP function which applies a **rectified linear unit (ReLU)** activation function and finally applies **softmax**.
* Building the **ouput layer**
* Defining the multilayer perceptron neural network architecture. This MLP has **1 input layer**, followed by **2 hidden layers** and finally the **output layer**.
* Setting the number of `epochs`, and using a regularized **cross-entropy** criterion.

* Implementing the `dropout`.

### MLP Summary

**Layer**          | **Shape** | **Neurons**
------------------ | --------- | -----------
Input              | 32x32x3   | 3072
Hidden Layer 1     | 1x2048    | 2048
Hidden Layer 2     | 1x2048    | 2048
Output             | 1x10      | 10

Dropout layer is applied after Input Layer (p<sub>1</sub>=0.1), Hidden Layer 1 (p<sub>2</sub>=0.5) and Hidden Layer 2 (p<sub>3</sub>=0.5).

**Training hyperparameters (w/dropout):**
* Epochs: 200
* Learning rate: 0.001
* L2 regularization parameter: 0.0001


### Results
**Results (w/dropout):**
Empirical test error: 43.76%
Number of test errors: 4376
Empirical training error: 13.53%
Number of training errors: 6765

**Results (with dropout):**
Empirical test error: 
Number of test errors: 
Empirical training error: 
Number of training errors: 