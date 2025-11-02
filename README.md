# Methods of Computational Intelligence

A university project exploring two fundamental neural network architectures: Multilayer Perceptrons (MLP) and Self-Organizing Maps (SOM). The work covered unsupervised clustering and visualization of multidimensional data using SOMs (including rectangular and hexagonal topologies), as well as supervised learning with MLPs, implementing backpropagation, gradient optimization, various activation functions, and regularization techniques to improve model performance.

## NN - MLP neural networks

This part explores **Multilayer Perceptron (MLP)** neural networks, covering key aspects of network design, training optimization, and model evaluation. The work focused on implementing core neural network mechanisms from scratch and analyzing their performance across various datasets.

Report: https://github.com/hoanganhlinh/MIO/blob/main/NN/NN___MLP_raport.pdf

### NN1 – Base Implementation

Developed the core MLP architecture with adjustable layers and neurons. Parameters were manually tuned to achieve optimal mean squared error (MSE) for regression datasets.

### NN2 – Backpropagation Implementation

Implemented **backpropagation** for training neural networks. Conducted experiments on batch vs. full-dataset updates to study convergence speed and training stability.

### NN3 – Gradient Optimization (Momentum & RMSProp)

Enhanced gradient descent with **momentum** and **RMSProp** methods. Compared their effects on convergence and model performance, identifying momentum as the most effective improvement.

### NN4 – Classification Tasks

Added **Softmax** output and **F-measure** loss function for classification problems. Tested the model on several datasets, showing improved results with Softmax activation.

### NN5 – Activation Functions

Integrated multiple activation functions: **sigmoid**, **tanh**, **ReLU**, and **linear**. Compared their performance for regression and classification tasks to determine optimal function choices for different problem types.

### NN6 – Overfitting and Regularization

Implemented **L2 regularization** and **early stopping** to prevent overfitting. Analyzed their effect on convergence and generalization, confirming their benefits for sparse and imbalanced datasets.

---

## KOH - Kohonen Networks (SOM)

This part explores **Self-Organizing Maps (SOM)**, also known as **Kohonen Networks**, applied to clustering and visualization of multidimensional data.

Report: https://github.com/hoanganhlinh/MIO/blob/main/KOH/KOH_raport.pdf

### KOH1 – Basic Kohonen Network

Implemented a standard rectangular SOM for clustering 2D and 3D datasets (Hexagon and Cube).

* Tested different neighborhood functions (Gaussian and Mexican Hat) and map dimensions.
* Evaluated models using the **v-measure** metric to assess clustering quality.
* Compared the influence of network parameters (grid size, neighborhood width, learning rate) on results.

### KOH2 – Hexagonal Kohonen Network

Extended the model to a **hexagonal topology** and tested it on more complex datasets:

* **HAR (Human Activity Recognition)** and **MNIST** handwritten digits.
* Compared rectangular and hexagonal grids using Gaussian and Mexican Hat functions.
* Analyzed clustering quality and discussed SOM performance on high-dimensional data.
