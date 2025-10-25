# mini-Project
 SignGuard – Automated Signature Forgery Detection System

An automated handwritten signature verification system using image processing and machine learning techniques to detect forged vs. genuine signatures with high accuracy.

 Overview

Manual signature verification is often slow, inconsistent, and prone to human error.
SignGuard automates this process by extracting distinctive features from scanned signatures and training a neural network to classify authenticity.

The system performs:

Image Preprocessing – Converts RGB signatures to grayscale, applies Gaussian blur, and uses Otsu thresholding for binarization.

Feature Extraction – Calculates nine handcrafted features:

Foreground pixel ratio

Normalized centroid (y, x)

Eccentricity

Solidity

Skewness (x, y)

Kurtosis (x, y)

Model Training – Uses a Multi-Layer Perceptron (MLP) built in TensorFlow/Keras.

Evaluation – Compares model accuracy
