---
title: Artificial Intelligence Project 2
date: 2024-03-02
---

The project explaining how to implement and learn a logistic regression model for multi-class classification based on the MNIST dataset using Numpy and Scikit-learn

<!--more-->
```
1. Overview
This report describes how Numpy and Scikit-learn can be used to implement and learn a logistic regression model for multi-class classification based on the MNIST dataset. It covers the data preprocessing, learning, and evaluation methods required for model training, and includes training parameters that can be adjusted by the user.

2. Implementation Method
- Library import : import numpy, sklearn.datasets, sklearn.model_selection, sklearn.preprocessing, matplotlib.pyplot to load, preprocess, build and evaluate, and visualize data.
- Set Argument Parser: Use argparse to set customization options; for example, you can customize the minibatch size and the maximum number of epoxies.
- Load and preprocess the MNIST dataset: Load the MNIST dataset using datasets.fetch_openml. Normalize the data, subtract the average of each pixel value. Transform label data for use in multi-class classification by one-hot encoding.
- Data Segmentation: Using training_test_split, we divide the data into training, validation, and test sets. First, we divide the entire data into training sets and temporary sets, and then we divide the temporary sets into validation sets and test sets again.
- Model creation and training: instantiate a logistic regression class to create a model; use training data to train the model; use verification data to evaluate model performance.
- Model Evaluation: Evaluate the final performance of the trained model using a test dataset. Outputs the test accuracy of the model.
- Visualize the results: use matplotlib.pyplot to visualize the first image data, which is useful for making sure that the data is loaded and preprocessed correctly.

3. Key Implementation Code Summary
- Argument Parser Settings: Set by receiving the mini batch size and maximum number of epoxies from the user.
- Data loading and preprocessing: Loads the MNIST dataset to perform normalization and one-hot encoding. Split the data into training, validation, and test sets.
- Model training: train the model using a logistic regression class; optimize the model's training process using mini-batch gradient descent and Early Stopping.
- Model Evaluation: Evaluate the performance of the model using a test set, and output accuracy.
- Visualize results: Visualize the first learned image to ensure that the data is processed correctly.

4. Conclusion
This method effectively builds and learns a logistic regression model to solve the multi-class classification problem. It increases the flexibility of the model by allowing the user to adjust the training parameters, and applies the Early Stopping technique to prevent overfitting and improve the generalization performance of the model. The data preprocessing and segmentation process ensures the quality of the data and accurately evaluates the performance of the final model.
```