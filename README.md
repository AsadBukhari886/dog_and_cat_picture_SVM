
# 🐶🐱 Dog vs. Cat Image Classifier using SVM

A binary image classification project that distinguishes between dog and cat images using classical machine learning techniques. Built with Python, Scikit-learn, OpenCV, and PIL.

## 📌 Project Overview

This project uses a **Support Vector Machine (SVM)** and **Logistic Regression** to classify grayscale images of dogs and cats based on their histogram features. It includes:
- Image preprocessing: resizing, grayscale conversion, histogram extraction, and Gaussian blur
- Manual label extraction from filenames
- Model training and probability-based prediction
- Results export in CSV format (Kaggle-style)

## 🧠 Model Summary

- **Model**: Linear SVM and Logistic Regression
- **Features**: Histogram of 64×64 grayscale, blurred images
- **Data**: Images should be placed in `../input/train/` and `../input/test/` (relative to the script)

## 🗂️ Files in this Repository

.
├── data.csv # (Optional) Local dataset preview or logs
├── dogsVScats.csv # Output predictions (id, label)
├── MSR-LA - 3467.docx # Related report or documentation (if any)
├── my_SVM.py # Main script for training and testing the model
├── readme[1].txt # Backup or rough readme version
├── tempCodeRunnerFile.py # Temporary VS Code runner file
└── README.md # This documentation



> **Note:** Image data (train/test images) must be stored locally in a path like `../input/train/` and `../input/test/`. These are not included in this repository.

## 🔧 Setup Instructions

Install required libraries:

```
pip install numpy pandas opencv-python scikit-learn pillow
Download and extract the Kaggle Dogs vs. Cats dataset, and place:

Training images in: ../input/train/

Test images in: ../input/test/

🚀 How to Run
Run the main script:


python my_SVM.py
This performs:

Label extraction from image filenames

Preprocessing: resize → grayscale → blur → histogram

Training with SVM / Logistic Regression

Prediction with probability calibration

CSV export of results in dogsVScats.csv

📊 Output Format
Sample dogsVScats.csv:


id,label
1,0.91
2,0.07
3,0.62
...
Where label is the confidence score that the image is a dog (1) or cat (0).

📈 Accuracy Evaluation (Optional)
The script includes a getResults() function that can be used to calculate accuracy on a validation split from the training set.

🧪 Technologies Used
Python

NumPy, Pandas

Scikit-learn (LinearSVC, LogisticRegression)

Pillow (PIL)

OpenCV

📄 License
This project is free to use for educational and non-commercial purposes.

🙋‍♂️ Author
Asad Bukhari
For queries or feedback, feel free to connect or raise an issue.
