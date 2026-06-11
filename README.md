# 🚗 Autonomous Vehicle Image Classification with Pixel Perturbation Attack and Defense

## 📌 Project Overview

This project demonstrates how Machine Learning can be used in autonomous vehicle vision systems to classify images and evaluate the impact of adversarial attacks on model performance.

Using the CIFAR-10 dataset as a simplified representation of real-world driving environments, the project investigates how small image modifications (pixel perturbations) can influence classification accuracy and how defense mechanisms can improve model robustness.

---

## 🎯 Objectives

* Classify images using traditional Machine Learning models.
* Extract meaningful image features using HOG (Histogram of Oriented Gradients).
* Simulate adversarial attacks through pixel perturbations.
* Analyze the effect of attacks on model confidence and accuracy.
* Implement defense mechanisms to improve robustness.
* Demonstrate the relevance of adversarial robustness in autonomous vehicle perception systems.

---

## 📂 Dataset

**Dataset:** CIFAR-10

The CIFAR-10 dataset contains 60,000 color images belonging to 10 classes:

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

Dataset Split:

* Training Images: 50,000
* Testing Images: 10,000

---

## 🔍 Feature Extraction

### HOG (Histogram of Oriented Gradients)

HOG is used to extract edge and shape-based features from images.

Benefits:

* Captures object boundaries and structural information.
* Reduces image dimensionality.
* Improves performance of traditional Machine Learning models.

Applications in Autonomous Vehicles:

* Lane detection
* Vehicle detection
* Traffic sign recognition
* Pedestrian detection

---

## 🤖 Machine Learning Models

The following models are trained and evaluated:

### 1. Logistic Regression

A simple and efficient linear classification algorithm.

### 2. Support Vector Machine (SVM)

Finds optimal decision boundaries between classes and performs well on high-dimensional feature spaces.

### 3. Random Forest

An ensemble learning method that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

---

## ⚠️ Adversarial Attacks (Pixel Perturbation)

Pixel perturbation refers to small modifications in image pixels that may be nearly invisible to humans but can significantly affect AI predictions.

### 1. Gaussian Noise

* Random noise added to image pixels.
* Simulates:

  * Rain
  * Fog
  * Low-light conditions
  * Camera sensor noise

### 2. Salt-and-Pepper Noise

* Random black and white pixels inserted into images.
* Simulates:

  * Camera transmission errors
  * Sensor malfunctions

### 3. Pixel Attack

* Random pixels are modified within the image.
* Demonstrates how small perturbations can confuse Machine Learning models and lead to incorrect classifications.

---

## 📊 Attack Analysis

For each attack, the following metrics are analyzed:

* Prediction before attack
* Prediction after attack
* Confidence score changes
* L2 Distance (amount of perturbation)

Visual outputs include:

* Original Image
* Attacked Image
* Perturbation Map

---

## 🛡️ Defense Mechanisms

### Gaussian Blur

Reduces image noise by smoothing pixel values before classification.

### Median Filtering

Removes isolated noisy pixels while preserving important image details.

### Anomaly Detection

Detects potential attacks by monitoring sudden drops in prediction confidence.

---

## 📈 Performance Evaluation

The project compares model performance under different noise levels.

Evaluation Metrics:

* Classification Accuracy
* Confidence Scores
* Accuracy vs Noise Level Analysis

Results demonstrate how image corruption affects model performance and how defense techniques help improve robustness.

---

## 🧠 Neural Network Extension

A Multi-Layer Perceptron (MLP) is implemented using PyTorch to explore deep learning-based classification and provide a foundation for future adversarial attack techniques such as:

* FGSM (Fast Gradient Sign Method)
* Gradient-Based Adversarial Attacks

---

## 🚘 Relevance to Autonomous Vehicles

Autonomous vehicles rely heavily on camera-based perception systems for decision-making.

Real-world conditions such as:

* Rain
* Fog
* Sensor noise
* Adversarial attacks

can alter image pixels and potentially cause misclassification.

This project demonstrates how pixel perturbations affect AI models and evaluates defense mechanisms that improve the reliability, safety, and robustness of autonomous driving systems.

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* OpenCV
* Matplotlib
* Scikit-Learn
* Scikit-Image
* PyTorch
* Google Colab

---

## 📷 Sample Outputs

* Baseline Model Accuracy
* Attack Visualizations
* Confidence Drop Analysis
* Accuracy vs Noise Graphs
* Defense Evaluation Results

---

## 🚀 Future Improvements

* CNN-Based Classification Models
* FGSM and PGD Adversarial Attacks
* Real Traffic Sign Datasets
* Sensor Fusion Techniques
* Advanced Defense Strategies

---

## 👩‍💻 Author

**Shravani Samala**

Machine Learning Project | Autonomous Vehicle Security & Adversarial Robustness
