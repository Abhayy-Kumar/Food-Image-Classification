# Food Image Classification

This repository contains a deep learning project that classifies images of 101 different foods. The project utilizes a pretrained MobileNetV2 model from TensorFlow/Keras and fine-tunes it with additional dense layers to achieve accurate food category predictions.

## Overview
The objective of this project is to build an image classification system that identifies the food present in a given image. We employ a TensorFlow/Keras pretrained MobileNetV2 model, which is further fine-tuned with additional fully connected layers to classify images into 101 food categories. The project also includes steps for data preparation, train-test splitting, model training with early stopping, and evaluation using confusion matrices and classification reports.

## Features
- **Data Preparation:** 
  - Downloads the Food-41 dataset from Kaggle.
  - Unzips and organizes images into a structured DataFrame.
- **Data Splitting & Augmentation:** 
  - Splits the dataset into training, validation, and testing sets.
  - Uses TensorFlow's `ImageDataGenerator` with MobileNetV2 preprocessing.
- **Modeling & Transfer Learning:** 
  - Leverages MobileNetV2 as a feature extractor (with frozen weights).
  - Adds two Dense layers and a softmax output layer to classify 101 food categories.
- **Training & Early Stopping:** 
  - Uses the Adam optimizer and categorical crossentropy loss.
  - Incorporates early stopping to prevent overfitting.
- **Evaluation & Visualization:** 
  - Evaluates the model on a test set.
  - Generates confusion matrices and classification reports.
  - Visualizes the confusion matrix using Seaborn and Matplotlib.


### Dataset link - https://www.kaggle.com/datasets/kmader/food41
