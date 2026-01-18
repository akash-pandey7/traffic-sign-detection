# 🚦 Traffic Sign Detection and Recognition System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Overview
The **Traffic Sign Detection and Recognition System** is a Deep Learning project designed to classify traffic signs into **43 distinct categories** (e.g., Stop, Speed Limit, Yield) with high accuracy. Built using **Python**, **TensorFlow/Keras**, and **OpenCV**, this system serves as a prototype for autonomous vehicle navigation and driver assistance systems (ADAS).

It achieves an accuracy of **~95%** on the [German Traffic Sign Recognition Benchmark (GTSRB)](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset) dataset.

---

## 🚀 Features
* **Deep Learning Model:** A custom Convolutional Neural Network (CNN) optimized for image classification.
* **High Accuracy:** Achieves >95% accuracy on test data.
* **Batch Prediction:** Includes a dedicated script (`run_batch_prediction`) to process multiple images from a folder at once.
* **Robust Preprocessing:** Handles image resizing, normalization, and one-hot encoding automatically.
* **Visualizations:** Generates confusion matrices, accuracy/loss graphs, and prediction grids.

---

## 📂 Project Structure
```bash
Traffic_Sign_Detection/
│
├── Data/                       # Dataset folder (GTSRB)
│   ├── Train/                  # Training images (0-42 folders)
│   ├── Test/                   # Test images
│   ├── Train.csv               # Training labels
│   └── Test.csv                # Test labels
│
├── models/                     # Saved models
│   └── traffic_sign_detection_gtsrb.h5
│
├── new_images/                 # Folder for testing new images
│   ├── sign1.png
│   └── sign2.jpg
│
├── traffic_sign_detection.ipynb # Main Jupyter Notebook for training
├── batch_prediction.py         # Script for batch testing
├── README.md                   # Project documentation
└── requirements.txt            # Python dependencies
```
# 🛠️ Tech Stack
* **Language**: Python

* **Libraries**: TensorFlow, Keras, NumPy, Pandas, Matplotlib, Scikit-learn, PIL (Pillow).

* **Dataset**: GTSRB (German Traffic Sign Recognition Benchmark).

# ⚙️ Installation & Setup
1. **Clone the repository** : 
```bash
git clone [https://github.com/akash-pandey7/traffic-sign-detection.git](https://github.com/akash-pandey7/traffic-sign-detection.git)
```
2. **Install Dependencies** : It is recommended to use a virtual environment.
```bash
pip install -r requirements.txt
```
3. **Dataset Setup**
* Download the GTSRB dataset from [here](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)
* Extract it into the `Data/` folder so that `Data/Train` and  `Data/Test` exist.