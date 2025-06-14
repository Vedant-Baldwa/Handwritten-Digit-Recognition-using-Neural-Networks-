# Handwritten Digit Recognition using Deep Learning

## 📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** to accurately recognize handwritten digits (0–9) from a large custom dataset of over **107,000 images**.

Unlike traditional MNIST-based solutions, this project uses a **custom dataset** with PNG images, providing a more robust and scalable approach.

---

## 🚀 Features

- Data preprocessing pipeline (alpha channel extraction + binarization)
- CNN architecture with:
  - 4 Convolutional layers + MaxPooling layers
  - Fully connected Dense layers
- Model evaluation using:
  - Test accuracy
  - Confusion matrix visualization
- Large-scale dataset handling (>107k images)
- Designed for **integration into a web application** (in progress 🚧)

---

## 🖥️ Tech Stack

- **Python 3.8+**
- **TensorFlow / Keras**
- **NumPy / Pandas**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## 📂 Dataset

- **Source:** Custom PNG dataset  
- **Size:** 107,730 images  
- **Classes:** 10 (digits 0–9)  
- **Image Size:** 28×28 pixels  
- **Input Shape:** (784,) after flattening

---

## 🏗️ Model Architecture

- Input Layer → Reshape to (28,28,1)
- **Conv2D(64, 3×3) + ReLU + MaxPooling**
- **Conv2D(32, 3×3) + ReLU + MaxPooling**
- **Conv2D(16, 3×3) + ReLU + MaxPooling**
- **Conv2D(64, 3×3) + ReLU + MaxPooling**
- **Flatten**
- **Dense(64) + ReLU**
- **Dense(10) → Output logits**

---

## 📝 Results

- **Training Accuracy:** 100%
- **Test Accuracy:** 100%
- **Confusion Matrix:** Perfect (no misclassifications)
![plots](https://github.com/Vedant-Baldwa/Handwritten-Digit-Recognition-using-Neural-Networks-/blob/9e2fe5594e14b55221a6fa503a689453577b24c0/results/graph.png)
![Confusion Matrix](https://github.com/Vedant-Baldwa/Handwritten-Digit-Recognition-using-Neural-Networks-/blob/9e2fe5594e14b55221a6fa503a689453577b24c0/results/Confusion%20Matrix.png)
![Prediction](![plots](https://github.com/Vedant-Baldwa/Handwritten-Digit-Recognition-using-Neural-Networks-/blob/9e2fe5594e14b55221a6fa503a689453577b24c0/results/Prediction.png)

---

## 🌐 Future Work — Web Application Integration

The next phase of this project will be to integrate the trained model into a **web application** to provide an interactive demo where users can upload their handwritten digit images and get real-time predictions.

Planned tech stack for web app:

- **Django** (backend framework)
- **TensorFlow SavedModel / TFLite** for serving the model
- **HTML / CSS / JS** for frontend interface

---

## 🔧 Setup Instructions

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/handwritten-digit-recognition.git
    cd handwritten-digit-recognition
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the notebook:
    ```bash
    jupyter notebook
    ```

---

## 🤝 Contributing

Contributions are welcome! If you’d like to add features (data augmentation, web app integration), feel free to fork the repo and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---
