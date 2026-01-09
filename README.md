# Facial Emotion Recognition System 🎭

A deep learning–based Facial Emotion Recognition System that detects and classifies human emotions from facial expressions using **Convolutional Neural Networks (CNN)** and **Transfer Learning** with **MobileNetV2**.  
The system works on both **static images** and **real-time webcam input**.

---

## 📌 Features
- Real-time emotion detection using webcam
- Emotion prediction from images
- Transfer Learning with MobileNetV2
- Trained on FER-2013 dataset
- Data augmentation for better accuracy
- Lightweight and efficient model

---

## 😊 Emotion Classes
The model classifies facial expressions into **7 emotions**:
- Angry 😡
- Disgust 🤢
- Fear 😨
- Happy 😊
- Sad 😢
- Surprise 😲
- Neutral 😐

---

## 🧠 Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- MobileNetV2 (Pre-trained model)
- FER-2013 Dataset

---

## 🗂️ Dataset
- **FER-2013** dataset
- Grayscale facial images of size **48×48**
- Dataset structure:
train/
├── angry/
├── disgust/
├── fear/
├── happy/
├── sad/
├── surprise/
└── neutral/

yaml
Copy code

---

## ⚙️ Model Architecture
- Base Model: **MobileNetV2** (pre-trained on ImageNet)
- Added Layers:
  - Global Average Pooling
  - Dense (ReLU)
  - Dropout
  - Dense (Softmax – 7 classes)

---

## 🔁 Workflow
1. Capture image or webcam frame
2. Detect face using OpenCV
3. Preprocess face (resize, normalize)
4. Feature extraction using MobileNetV2
5. Emotion classification
6. Display predicted emotion

---

## 📊 Results
- Achieved **~85–90% accuracy**
- Best performance on:
  - Happy
  - Surprise
- Works smoothly in real-time on standard hardware
