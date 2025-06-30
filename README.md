# ASL Letter Detection Using Computer Vision

This project focuses on detecting American Sign Language (ASL) letters from hand gesture images using MediaPipe for hand landmark extraction and a Random Forest Classifier for classification. The model achieved an impressive 97.4% accuracy on the test set.

## Introduction

The goal of this project is to build a system that can recognize individual letters of ASL (A–Z) from static hand gesture images. It can also predict entire words if a sequence of ASL letter images is provided.

* This system can be used for:

* Real-time gesture-to-text applications

* Education tools for learning ASL

* Accessibility enhancement for deaf and hard-of-hearing individuals

## Technologies Used
* MediaPipe – for hand landmark detection

* Random Forest Classifier – for classification of hand gestures

* scikit-learn – for model training, testing, and evaluation

* OpenCV – for image processing

* Pandas, NumPy – for data handling

* kaggle Notebook – for development and testing

## Dataset
- Dataset: American Sign Language (ASL) A–Z letter image dataset

- Source: [Kaggle ASL Dataset](https://www.kaggle.com/datasets/krishnapaanchajanya/american-sign-language-asl)

- Structure: Images categorized in folders A to Z

- Preprocessing: Only images with valid hand landmarks (detected using MediaPipe) are used

## How It Works
* Load image data from folders A to Z.

* Use MediaPipe to extract 21 hand landmarks (x and y coordinates).

* Combine x and y coordinates into a single feature vector.

* Train a Random Forest classifier on the extracted features.

* Use the trained model to:

- Predict the ASL letter from a given hand gesture image

- Predict entire words from a sequence of letter images

## Results
Model Accuracy: ~97.4% on test data

Classifier: Random Forest
