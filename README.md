# CNN-Based-Handwritten-Digit-Recognition-on-Edge-Device

## 📌 Project Overview
This project implements a Convolutional Neural Network (CNN) to classify and predict handwritten digits (0–9) using the MNIST dataset. The built model is then deployed on an edge device(Android phone) and live testing of hand written digits is implemented.

---


## 🔗 Project Link
https://snigdha-c.github.io/CNN-Based-Handwritten-Digit-Recognition-on-Edge-Device/

---

## 🔄 Project Pipeline
<img width="1089" height="520" alt="image" src="https://github.com/user-attachments/assets/f357e334-0dab-417d-8479-c9b3d907577d" />

---

## 📂 Dataset
- **Dataset:** MNIST Handwritten Digits  
- **Training samples:** 60,000  
- **Test samples:** 10,000  
- **Image size:** 28 × 28 pixels (grayscale)  
- **Classes:** 10 (digits 0–9)  
---

## ⚙️ Technologies Used
- Python  
- NumPy  
- TensorFlow / Keras
- ONNX
- Quantization
- HTML
---

## 💻 Implementation
- Built a **Convolutional Neural Network (CNN)** using TensorFlow/Keras to classify MNIST digits.
- Converted the trained TensorFlow model to **ONNX format** for cross-framework compatibility.
- **Post-Training Quantization** was applied using ONNX Runtime to convert model weights from FP32 to INT8 for efficient edge inference.
- Deployed the model on an **Android device** and performed inference using **ONNX Runtime.**
- Implemented **live handwritten digit testing on the phone.**  
---

## 🛠️ Model Architecture
- **Input Layer:** 28 × 28 × 1 neurons 
- **Hidden Layers:**
  - Conv2D (28 filters, 3×3 kernel) with ReLU activation
  - MaxPooling2D (2×2)
  - Conv2D (28 filters, 3×3 kernel) with ReLU activation
  - MaxPooling2D (2×2)
  - Flatten
  - Dense layer with 64 neurons and ReLU activation
- **Output Layer:** 10 neurons with Softmax activation  
- **Loss Function:** Sparse Categorical Crossentropy  
- **Optimizer:** Adam  
---

## 📊 Model Performance
- **Training Accuracy:** 99.19%  
- **Test Accuracy:** 98.76%
- **Test Accuracy of ONNX Quantized model:** 98.76%
- **Original model size:** 211.3505859375 KB
- **Quantized model size:** 64.8544921875 KB
---

## 📱 Live Prediction Results Implemented on Edge Device

<img width="1125" height="577" alt="image" src="https://github.com/user-attachments/assets/a6c89689-baf4-48b2-8f5a-ccbbfb2ee1c7" />

<img width="812" height="601" alt="image" src="https://github.com/user-attachments/assets/ec658603-3ebd-41e1-a68b-daeb5130dffb" />

<img width="843" height="574" alt="image" src="https://github.com/user-attachments/assets/dd9b3b41-cf6a-4ff2-9dab-7563e5c6e664" />

---

## 📈 Key Observations
- CNNs are effective for handwritten digit recognition.
- ONNX conversion maintains model consistency, preserves the model structure and predictions.
- The ONNX Runtime allows the model to run inference directly on the Android device without relying on cloud computation.
- Quantization significantly reduces model size.
- Real-time handwritten digits can differ from MNIST samples in thickness, alignment, or scale, which can affect prediction quality.
- The deployed model can predict blurred images as well as numbers written in different styles as observed in the "Special Case Predictions".
- There is space for improvement as model can sometimes give incorrect predictions.
---

## ✅ Conclusion
- **End-to-end ML pipeline from training to deployment**  
The project demonstrates the complete workflow from model training and optimization to deployment and inference on an edge device.

---

## ⚡ Future Work
- Working on applying similar techniques to Hand Sign Language Detection Project.
- Improve performance and minimize incorrect predictions.
- Explore deployment on other edge devices such as raspberry pi.

---
  
