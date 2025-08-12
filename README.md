# Overfitting Detection and Regularization with PyTorch

This repository contains two separate projects that explore and address the problem of **overfitting** in neural networks. Each project is implemented in a Jupyter Notebook and uses the **FashionMNIST** dataset for a common learning task.

-----

## 📁 Project Structure

  - **`nn_overfitting_validation.ipynb`**: This notebook focuses on **detecting** overfitting. It trains a neural network and monitors its performance on both a **training set** and a **validation set**. By plotting and comparing the loss on both sets, you can identify the point where the model begins to memorize training data, causing its performance on new, unseen data to degrade.

  - **`nn_overfitting_regularization.ipynb`**: This notebook is designed to **mitigate** overfitting. It modifies the neural network's architecture to include **regularization techniques**, such as **Dropout** and/or **L2 regularization** (suggested techniques). The goal is to improve the model's ability to generalize to new data, thereby reducing overfitting.

-----

## 🚀 Getting Started

To run these projects, you need to have the following libraries installed. You can install them using `pip`:

```bash
pip install torch torchvision matplotlib
```

### How to Run

1.  Open the Jupyter Notebook files.
2.  Run the cells in each notebook sequentially.
3.  The output of each project, including loss plots and performance metrics, will be displayed directly in the notebook.

## 📊 Analysis of Results

### `nn_overfitting_validation` Project

  - **Goal**: To identify overfitting.
  - **Expected Outcome**: The training loss plot is expected to continue decreasing, while the validation loss plot will eventually stop decreasing and may even start to increase. This divergence is a key sign of overfitting.

### `nn_overfitting_regularization` Project

  - **Goal**: To prevent overfitting.
  - **Expected Outcome**: After adding regularization techniques, the plots for both training and validation loss should show a more aligned trend. The validation loss should not increase as rapidly, indicating that the model's generalization ability has improved.

## 📝 Technical Notes

  - **Dataset**: The **FashionMNIST** dataset is used for an image classification task.
  - **Preprocessing**: The images are normalized before being fed to the model.
  - **Model**: A simple multi-layer neural network is implemented in both notebooks.
  - **Metrics**: Loss and accuracy are used to evaluate the model's performance.
