# 🖼️ CIFAR-10 Image Classification with Transfer Learning

This project implements **image classification** on the **CIFAR-10 dataset** using **Transfer Learning** with the **MobileNetV2** model. The goal is to classify images into **10 categories** such as airplanes, cars, birds, cats, deer, dogs, frogs, horses, ships, and trucks.

## 📂 Dataset Information
The **CIFAR-10 dataset** is a widely used dataset in machine learning research, containing:
- **60,000** color images of **32x32 pixels**.
- **10 classes** with **6,000 images per class**.
- Pre-split into **50,000 training** and **10,000 testing** images.

## 🔥 Project Overview
### ✨ **Why Transfer Learning?**
Instead of training a deep learning model from scratch, we leverage **pre-trained models** (MobileNetV2) trained on **ImageNet** to improve performance and reduce training time.

### 🛠️ **Approach**
1. **Load the CIFAR-10 dataset** and normalize the pixel values.
2. **Use a pre-trained MobileNetV2 model**, removing the top layers.
3. **Freeze the base layers** to retain useful image features.
4. **Add new dense layers** for CIFAR-10 classification.
5. **Train the model** on the dataset and evaluate accuracy.


**Final Test Accuracy: 34.78%**

> 🧐 The accuracy is relatively low because CIFAR-10 is a **challenging dataset** for models trained with **ImageNet** features. Fine-tuning more layers and training longer would improve results.
