# Handwritten Digit Recognition using CNN and RNN

A Deep learning project for handwritten digit classification using CNN and RNN models implemented with PyTorch.

The project trains both models on the MNIST handwritten digit dataset and compares their classification performance using accuracy and confusion matrices.

## 📌 Project Overview

Handwritten digit recognition is a fundamental computer vision problem where a model learns to identify digits from handwritten images.

In this project, two different deep learning approaches are implemented:

- **CNN** for learning spatial features from images
- **RNN** for processing the image as a sequence

The performance of both models is evaluated and compared on the test dataset.

## 🎯 Objectives

- Understand image classification using deep learning
- Implement a CNN using PyTorch
- Represent image data as a sequence for RNN processing
- Train and evaluate both models
- Compare CNN and RNN classification performance
- Analyze predictions using confusion matrices

## 🧠 Models Implemented

### 1. Convolutional Neural Network (CNN)

The CNN processes the handwritten digit images while learning spatial features through convolution and pooling operations.

### CNN Architecture
```text
Input Image (28 × 28)
        ↓
Convolution Layer
        ↓
Max Pooling
        ↓
Convolution Layer
        ↓
Max Pooling
        ↓
Convolution Layer
        ↓
Max Pooling
        ↓
Flatten
        ↓
Fully Connected Layer
        ↓
ReLU
        ↓
Output Layer
        ↓
10 Digit Classes
```
The CNN contains convolutional layers with 32, 64, and 128 filters, followed by fully connected layers for classification.

### 2. Recurrent Neural Network (RNN)

For the RNN, each handwritten digit image is converted into a sequence before being given to the network.

The original image has the shape:
28 × 28

It is represented as:
28 time steps × 28 features

The RNN processes these sequential inputs and uses the learned representation for digit classification.

### RNN Workflow
```text
Input Image
     ↓
Convert Image into Sequence
     ↓
RNN
     ↓
Hidden State
     ↓
Fully Connected Layer
     ↓
10 Digit Classes
```
### 📊 Results

The models were evaluated on the test dataset.

Model	Test Accuracy
CNN	99.13%
RNN	96.16%

The CNN and RNN predictions were further analyzed using confusion matrices.
The confusion matrices show the number of correct and incorrect predictions for each digit class.

### 🔬 Project Workflow
```text
                MNIST Dataset
                      ↓
              Data Preprocessing
                      ↓
                Data Loading
                      ↓
          ┌───────────┴───────────┐
          ↓                       ↓
         CNN                     RNN
          ↓                       ↓
      Training                 Training
          ↓                       ↓
     Prediction              Prediction
          ↓                       ↓
      Evaluation              Evaluation
          ↓                       ↓
          └───────────┬───────────┘
                      ↓
              Performance
               Comparison
                      ↓
          Confusion Matrices
```
### 🛠️ Technologies Used
Python
PyTorch
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn

### 📚 Key Learning Outcomes

Through this project, I learned and implemented:

- Image classification using PyTorch
- CNN architecture for image data
- Convolution and pooling operations
- RNN-based sequence processing
- Converting image data into sequential input
- Model training and evaluation
- Accuracy calculation
- Confusion matrix analysis
- Comparison of different neural network architectures

### 🔮 Future Improvements

- Experiment with different CNN architectures
- Tune hyperparameters such as learning rate and batch size
- Add data augmentation
- Experiment with LSTM and GRU architectures
- Compare training time between CNN and RNN
- Add a real-time handwritten digit prediction interface
- Deploy the trained model as a web application

### 👩‍💻 Author
Utpala Polavarapu
