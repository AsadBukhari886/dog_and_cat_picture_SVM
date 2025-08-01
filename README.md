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

## 🗂️ Project Structure

dog_and_cat_picture_SVM/
├── input/
│ ├── train/ # Contains training images (e.g., dog.123.jpg, cat.456.jpg)
│ ├── test/ # Contains testing images for prediction
├── my_SVM.py # Main script for training and testing
├── results.csv # Output predictions (id, label)
└── README.md # Project documentation

perl
Copy
Edit

## 🔧 Installation & Setup

Ensure you have Python 3 installed and run the following to install required libraries:

```bash
pip install numpy pandas opencv-python scikit-learn pillow
Place the dataset under the input/ folder:

Training images go into input/train/

Testing images go into input/test/

You can use the Kaggle Dogs vs. Cats dataset.

🚀 How to Run
To train the model and generate predictions:

bash
Copy
Edit
python my_SVM.py
The following steps occur:

Label Extraction: Images with filenames containing "dog" are labeled 1, otherwise 0.

Preprocessing:

Convert to grayscale

Resize to 64x64

Apply Gaussian blur

Extract histogram features

Model Training:

Trains an SVM or Logistic Regression on all training data

Prediction:

Runs the trained model on test images

Outputs results to results.csv in (id, label) format

📊 Output Format
The prediction results are saved as:

csv
Copy
Edit
id,label
1,0.89
2,0.12
3,0.96
...
Where label is the model's confidence score for the "dog" class.

📈 Accuracy Evaluation
The script includes a getResults() function to evaluate predictions on a held-out set by comparing predicted probabilities against actual labels and calculating the classification accuracy.

🧪 Technologies Used
Python

Scikit-learn (LinearSVC, LogisticRegression)

Pillow (PIL) for image manipulation

OpenCV for preprocessing

NumPy / Pandas for numerical operations

📝 License
This project is open-source and free to use for educational or research purposes.

🙋‍♂️ Author
Asad Bukhari
Feel free to reach out for questions or collaboration!
