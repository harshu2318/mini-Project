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



How to Run

Clone the repository

git clone https://github.com/your-username/signguard.git
cd signguard


Install required libraries

pip install numpy scipy pandas matplotlib scikit-image tensorflow==1.15 keras


Set your dataset path

Update the base_path variable in the script to the folder containing your signature dataset (with <person> and <person>_forg subfolders).

Run the script

python sign_detection.py


When prompted:

Enter the person ID (e.g., 682)

Provide the path of the test signature image

The script will:

Automatically generate training/testing CSVs

Train the model

Print training & testing accuracy

Indicate if the given signature is genuine ✅ or forged ❌
