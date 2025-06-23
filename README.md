# classify-images-of-cats-and-dogs

This project builds a machine learning model that classifies pet images as either cats or dogs, using SVM (Support Vector Machine) after applying PCA for dimensionality reduction. A simple and intuitive Gradio interface allows users to upload images and get instant predictions.

# Dataset

Dataset used: Oxford-IIIT Pet Dataset

Classes: Cats & Dogs (12 cat breeds vs other dog breeds)

Custom limit per class: 200 images (adjustable)

# Features

Image preprocessing (resizing and flattening)

Dimensionality reduction using PCA

Classification using SVM (RBF Kernel)

Real-time predictions using Gradio

GUI to interactively upload and classify images

Accuracy ~85% with balanced dataset

# Model Pipeline

Load Images → Resize & Flatten → PCA → SVM Classifier → Save Model

# Gradio App

Once the model is trained and saved, launch the app with:

python app.py

The app will open a web interface where you can upload an image:

# Upload an image (jpg, png)

# Get instant classification: 🐱 Cat or 🐶 Dog

# Requirements

Install dependencies with:

pip install -r requirements.txt

# File Structure
project/

│

├── code + GUI.ipynb         # Training SVM with PCA and use Gradio for user interface

├── svm_model_pca.pkl       # Saved trained SVM model

├── pca_model.pkl           # Saved PCA transformer

├── requirements.txt

└── README.md

# Classification Report:

Accuracy: 0.85

