# 👕 Fashion-MNIST Image Classification using VGG16

<p align="center">
Deep Learning • Transfer Learning • PyTorch • Computer Vision
</p>

<p align="center">
📊 Dataset: Fashion-MNIST | 🧠 Model: VGG16 | ⚡ Framework: PyTorch
</p>

---

## 📌 Project Overview

This project implements an **image classification model** using **transfer learning with the VGG16 architecture** to classify clothing images from the **Fashion-MNIST dataset**.

The goal is to demonstrate how **pretrained deep learning models** can be adapted to new datasets using **PyTorch**.

The model learns to classify images into **10 clothing categories** such as T-shirt, Dress, Sneaker, Bag, etc.

---

## 📊 Dataset

The **Fashion-MNIST dataset** is a widely used benchmark dataset for machine learning.

**Dataset Features**

* 70,000 grayscale images
* Image size: **28 × 28 pixels**
* **10 clothing categories**
* 60,000 training images
* 10,000 testing images

**Classes**

| Label | Category      |
| ----- | ------------- |
| 0     | T-shirt / Top |
| 1     | Trouser       |
| 2     | Pullover      |
| 3     | Dress         |
| 4     | Coat          |
| 5     | Sandal        |
| 6     | Shirt         |
| 7     | Sneaker       |
| 8     | Bag           |
| 9     | Ankle Boot    |

---

## 🧠 Model Architecture

The project uses **VGG16**, a deep convolutional neural network pretrained on **ImageNet**.

### Transfer Learning Steps

1. Load pretrained **VGG16**
2. Freeze convolutional feature layers
3. Replace classifier layers
4. Train new fully connected layers

### Custom Classifier

```
Input (25088)
   ↓
Linear (1024)
   ↓
ReLU
   ↓
Dropout
   ↓
Linear (512)
   ↓
ReLU
   ↓
Dropout
   ↓
Linear (10 classes)
```

---

## ⚙️ Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Pandas
* Matplotlib

---

## 🔄 Project Workflow

1️⃣ Load Dataset
2️⃣ Visualize Sample Images
3️⃣ Data Preprocessing
4️⃣ Custom PyTorch Dataset
5️⃣ Load Pretrained VGG16
6️⃣ Modify Classifier
7️⃣ Train the Model
8️⃣ Evaluate Performance

---

## 📈 Model Training

* Loss Function: **CrossEntropyLoss**
* Optimizer: **Adam**
* Learning Rate: **0.001**
* Epochs: **100**

---

## 📊 Model Evaluation

The model is evaluated on the **test dataset** using classification accuracy.

```
Test Accuracy: XX%
```

*(Replace with your actual result)*

---

## 📂 Repository Structure

```
fashion-mnist-classification-vgg16
│
├── notebook
│   └── fashion_mnist_vgg16.ipynb
│
├── images
│   └── sample_images.png
│
└── README.md
```

---

## 🚀 Future Improvements

* Use **ResNet or EfficientNet**
* Apply **data augmentation**
* Fine-tune more layers
* Add **training accuracy & loss plots**
* Hyperparameter optimization

---

## ⭐ If you found this project helpful, consider giving it a star!
