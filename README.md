# ResNet-34 on CIFAR-10 for Image Classification

## 📌 Project Overview
This project implements **ResNet-34**, a deep residual neural network, for **image classification** on the **CIFAR-10 dataset** using **TensorFlow and Keras**.
The model leverages **data augmentation**, **residual blocks**, and **modern training techniques** to achieve high accuracy on the dataset.

---

## 📂 Dataset & Preprocessing
- **Dataset:** [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)
- **Classes:** 10 (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
- **Image Size:** 32×32 pixels
- **Preprocessing:**
  - Normalization: `rescale=1./255`
  - Train/Validation Split: **80/20**
- **Data Augmentation:**
  - Random horizontal flips
  - Width and height shifts

---

## 🧠 Model Details
- **Architecture:** ResNet-34 implemented using **Keras Functional API**
- **Key Components:**
  - Residual blocks with skip connections
  - Batch normalization & ReLU activation
- **Loss Function:** `categorical_crossentropy`
- **Optimizer:** `Adam`
- **Metrics:** `accuracy`

---

## ⚙️ Training Configuration
- **Epochs:** 10
- **Batch Size:** 64
- **Callbacks:**
  - `ModelCheckpoint` – Saves the best model during training
- **Hardware:** GPU recommended for faster training

---

## 📊 Results

| Metric             | Value |
|--------------------|-------|
| Training Accuracy  | *71%* |
| Testing Accuracy| *70%* |

### Performance Visualizations
- **Accuracy & Loss Curves**
![Accuracy Plot](images/Accuracy Plot.jpeg)
![Loss Plot](images/loss.png)

- **Confusion Matrix**
![Confusion Matrix](images/confusion_matrix.png)

- **Classification Report**
              precision    recall  f1-score   support

           0       0.86      0.61      0.71      1000
           1       0.85      0.92      0.88      1000
           2       0.62      0.61      0.62      1000
           3       0.51      0.50      0.51      1000
           4       0.69      0.65      0.67      1000
           5       0.80      0.40      0.53      1000
           6       0.50      0.96      0.66      1000
           7       0.92      0.58      0.71      1000
           8       0.78      0.89      0.83      1000
           9       0.80      0.88      0.84      1000

    accuracy                           0.70     10000
   macro avg       0.73      0.70      0.70     10000
weighted avg       0.73      0.70      0.70     10000

## 🚀 Installation & Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/MuhammadMuaaz9/cifar10-ResNet34.git

### 2️⃣ Install Dependencies

👨‍💻 Author Muhammad Muaaz
