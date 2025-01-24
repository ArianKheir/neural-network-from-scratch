# Neural Network Implementation for MNIST Classification

This project implements a neural network to classify the MNIST dataset (handwritten digits) without using any premade models or libraries like pytorch. The code is written in Python and organized in a Jupyter Notebook for easy understanding and execution. Each part of the code is thoroughly explained with comments above it to guide you through the logic and implementation.

---

## Setup Instructions

### 1. Download the MNIST Dataset
1. Download the MNIST dataset file `mnist.npz` from [this link](https://storage.googleapis.com/tensorflow/tf-keras-datasets/mnist.npz).
2. Place the downloaded `mnist.npz` file **in the same directory** as the Jupyter Notebook (`neural network.ipynb`).

---

### 2. Install Required Libraries
Ensure you have the following Python libraries installed:
- `numpy`
- `matplotlib`
- (Optional) `Jupyter Notebook` or `JupyterLab` for running the notebook.

Install them using:
```bash
pip install numpy matplotlib notebook
```
---
### 3. Run the Jupyter Notebook
1. Open a terminal or command prompt.
2. Navigate to the folder where the notebook and the MNIST dataset are located.
3. Start the Jupyter Notebook server:
```bash
jupyter notebook
```
4. Open neural network.ipynb in your browser.
---
## How to Use the Code
The notebook is divided into several sections, and each section is explained with comments above the code for better understanding. Here's the structure of the notebook:
1. Data Loading and Preprocessing
   - What it does: Loads the MNIST dataset, flattens and normalizes the images, and one-hot encodes the labels.
   - What you need to do: Ensure mnist.npz is in the correct location.
2. Neural Network Functions
   - Functions like `initialize_parameters`, `forward_propagation`, `backward_propagation`, and `update_parameters` are implemented to train the network step-by-step.
   - Each function has a detailed explanation of how it works and its role in the training process.
3. Training the Model
   - The `train_model` function orchestrates the entire training process.
   - You can adjust hyperparameters like:
       - `epochs`: Number of iterations over the training data.
       - `learning_rate`: Step size for gradient descent.
       - `mini_batch_size`: Number of examples per batch.
       - `keep_prob`: Dropout probability to prevent overfitting.
       - `lambda_`: Regularization strength.
   - Default values are set to reasonable defaults, but you can experiment with them.
4. Testing the Model
   - The `test_model` function evaluates the trained network on the test data.
   - Accuracy is printed as a percentage
---
## Features of the Code
1. Step-by-Step Implementation:
   - The notebook breaks down the neural network training process, including gradient descent, backpropagation, and parameter updates.
2. Customizable Architecture:
   - You can modify the number of layers and neurons in `layer_dims` to explore different architectures.
3. Hyperparameter Tuning:
   - All key hyperparameters(e.g. learning rate, epochs, mini-batch size) are adjustable for experimentation.
4. Detailed Explanations:
   - Every part of the code includes comments and explanations to help beginners understand the concepts behind the implementation.
---
## Project Directory Structure
``` graphql
project_folder/
├── mnist.npz         # MNIST dataset file (to be downloaded and placed here)
├── neural network.ipynb     # Jupyter Notebook with neural network implementation
└── README.md         # This file
```
---
## How to Contribute
If you have suggestions or improvements, feel free to fork the repository, make changes, and submit a pull request.

---
## Acknowledgments
This project uses the MNIST dataset, a widely recognized dataset for handwritten digit recognition. Thanks to Yann LeCun and his collaborators for making it available.

---
## License
This project is open source and available for every one

---
