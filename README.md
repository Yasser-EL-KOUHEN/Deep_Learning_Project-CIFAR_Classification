# Deep Learning for CIFAR Image Classification

This repository contains two projects focused on **image classification using deep learning**, each using a different deep learning framework and dataset:

* **TensorFlow on CIFAR-4**
* **PyTorch on CIFAR-100**

---

## 🔹 Project 1: CIFAR-4 Classification with TensorFlow

### ✅ Status: Complete

### 📌 Overview

Classifies images into four classes: **Bird, Cat, Frog, Horse** using various deep learning architectures:

* Multi-Layer Perceptron (MLP)
* Convolutional Neural Network (CNN)
* Transfer Learning with ResNet-50

### 🧾 Dataset: CIFAR-4

* Derived from CIFAR-10 (4 classes only)
* 24,000 RGB images of size 32×32

### 🔄 Preprocessing

* Normalization to `[0, 1]`
* One-hot encoding for labels
* Data augmentation: rotation, flipping, shifting

### 🧠 Models & Performance

| Model        | Train Accuracy | Test Accuracy |
| ------------ | -------------- | ------------- |
| MLP          | \~59%          | \~56%         |
| CNN          | \~82%          | \~80%         |
| ResNet-50 TL | \~98%          | \~95%         |

### ▶️ How to Run

```bash
pip install tensorflow numpy matplotlib scikit-learn
```

Notebook: `TENSORFLOW_CIPHAR4.ipynb`

---

## 🔹 Project 2: CIFAR-100 Classification with PyTorch

### ⚠️ Status: In Progress

### 📌 Overview

Initial implementation of a CNN-based classifier for **100-object categories** from CIFAR-100 using **PyTorch**. Includes a baseline CNN and a ResNet-18 model.

### 🧾 Dataset: CIFAR-100

* 50,000 training images, 10,000 test images
* 100 distinct classes (RGB 32x32)

### 🔄 Preprocessing

* Data augmentation: random cropping, horizontal flip
* Normalization:

  * Mean: `(0.5071, 0.4867, 0.4408)`
  * Std: `(0.2675, 0.2565, 0.2761)`

### 🧠 Models & Performance (Initial)

| Epoch | Train Acc (%) | Test Acc (%) |
| ----- | ------------- | ------------ |
| 1     | 10.47         | 12.15        |
| 10    | 22.75         | 22.86        |

Notebook: `Pytorch_CIPHAR100.ipynb`

### ▶️ How to Run

```bash
pip install torch torchvision matplotlib numpy
```

---

## 📁 Repository Structure

```
Deep_Learning_Project-CIFAR_Classification/
│
├── TENSORFLOW_CIPHAR4.ipynb      # CIFAR-4 project (TensorFlow, complete)
├── Pytorch_CIPHAR100.ipynb       # CIFAR-100 project (PyTorch, in progress)
└── README.md                     # Project description
```

---

## 🔧 Future Improvements

* ✅ Finalize ResNet training for CIFAR-100
* ✅ Implement learning curves and confusion matrices
* 🔜 Add comparative plots for both projects
* 🔜 Evaluate training time and efficiency across frameworks
