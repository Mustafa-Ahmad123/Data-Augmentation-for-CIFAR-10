# CIFAR-10 Image Classification Using CNN and Inception Module

## Project Overview
This project focuses on developing a lightweight Convolutional Neural Network (CNN) for image classification using the CIFAR-10 dataset. The model is trained from scratch without pretrained weights and incorporates an Inception-style module to extract features at different spatial scales while maintaining the assignment's constraint of fewer than one million trainable parameters.

## Methodology
The project explores different data augmentation techniques, including rotation, brightness and contrast adjustment, occlusion, and grayscale transformation, to investigate their effects on classification accuracy and robustness. Model performance is evaluated using validation data, clean test images, and shifted test images containing different types of corruption.

## Model Evaluation
Multiple random seeds are used to assess the consistency of model performance. Error analysis is conducted using classification reports, confusion matrices, and misclassified examples to identify common prediction errors. The model is also evaluated on an unseen Gaussian-noise corruption to examine its ability to generalize to data variations not included in training.

## Test-Time Augmentation
Test-Time Augmentation (TTA) is implemented by averaging predictions from original and horizontally flipped test images. Its effect on classification accuracy and inference time is compared with standard inference.

## Technologies
- Python
- TensorFlow and Keras
- NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Kaggle Notebooks and Jupyter

## Objective
The objective is to develop an efficient image classification model and analyze how architectural design, data augmentation, and inference-time techniques affect classification performance and robustness to image corruptions.

## Results
The repository includes experiments and evaluation results for different augmentation strategies, clean and shifted test accuracy, hidden-corruption testing, error analysis, and Test-Time Augmentation. The results help illustrate the strengths and limitations of a lightweight CNN under different testing conditions.
