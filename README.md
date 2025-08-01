# 🐶🐱 Dog vs. Cat Image Classifier using SVM

A binary image classification project that distinguishes between dog and cat images using classical machine learning techniques. Built with Python, Scikit-learn, OpenCV, PIL, and SVM from scratch.

## 📌 Project Overview

This project implements a pipeline to classify images of dogs and cats using:
- Traditional ML models: **Support Vector Machine (SVM)** and **Logistic Regression**
- Image preprocessing: resizing, grayscale conversion, histogram extraction, and Gaussian blur
- Custom training and prediction scripts
- CSV output for label predictions (e.g., suitable for Kaggle format)

## 🧠 Model Summary

- **Model**: Linear SVM (via `sklearn.svm.LinearSVC`) and Logistic Regression
- **Feature Extraction**: Histogram values of 64x64 grayscale images
- **Training Data**: Custom labeled images with filenames containing either "dog" or "cat"
- **Testing Data**: Unlabeled images used for prediction and output


