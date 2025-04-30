 ## Classification with Neural Networks

## Overview

This repository contains my implementation of a **feed-forward neural network classifier** in Python and Keras, trained on the Fashion-MNIST dataset. It closely follows the tutorial by The Clever Programmer but adapts the code structure, adds exploratory analysis, and includes my own experiments with layer sizes, activations, and training hyperparameters to improve performance.

- **Tutorial source:** https://thecleverprogrammer.com/2022/01/10/classification-with-neural-networks-using-python/  
- **My Kaggle notebook:** https://www.kaggle.com/code/rawsheed91/classification-with-neural-networks-using-python

---

## Project Structure

```
├── README.md                # this file
└── classification-with-neural-networks-using-python.ipynb     # main Jupyter notebook with full workflow
```

---

## Key Components

### 1. Data Loading & Preprocessing  
- Loads **Fashion-MNIST** directly via Keras.  
- Normalizes pixel values to [0,1].  
- Splits into train/validation/test sets.  

### 2. Model Architecture  
- **Input:** 28×28 flattened to 784 neurons.  
- **Hidden layers:**  
  - Dense(300) + ReLU  
  - Dense(100) + ReLU  
- **Output layer:** Dense(10) + Softmax  

### 3. Training  
- Loss: Categorical cross-entropy  
- Optimizer: Adam  
- Metrics: Accuracy  
- Validation split for early stopping  

### 4. Evaluation & Visualization  
- Plots of loss and accuracy over epochs.  
- Confusion matrix on test set.  
- Sample predictions visualized alongside true labels.  

---

## How to Run

1. **Clone the repo**  
   ```bash
   git clone https://github.com/OyewoleRasheed/Classification-with-Neural-Networks-using-Python.git
   cd Classification-with-Neural-Networks-using-Python
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**  
   ```bash
   jupyter notebook classification-with-neural-networks-using-python.ipynb
   ```

---

## Results

- Achieved **~88% test accuracy**.  
- Visual inspection shows misclassifications occur between similar garment types (e.g., Sneaker vs. Sandal).

---

## Acknowledgments

This project is based on and inspired by the excellent tutorial by **The Clever Programmer**:  
https://thecleverprogrammer.com/2022/01/10/classification-with-neural-networks-using-python/

---
