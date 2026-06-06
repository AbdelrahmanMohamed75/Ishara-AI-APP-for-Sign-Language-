# 🤟 AI-Powered American Sign Language (ASL) Recognition System

An AI-powered American Sign Language (ASL) recognition system that detects and classifies hand gestures representing the 26 English alphabet letters (A-Z). The project combines computer vision, hand landmark extraction, deep learning, and YOLO-based real-time gesture recognition to assist communication between deaf and hearing individuals.

---

## 🎯 Project Objective

Communication barriers between deaf and hearing individuals remain a challenge in many environments.

The goal of this project is to develop an intelligent ASL recognition system capable of:

- Detecting hands in images and videos.
- Extracting meaningful hand landmarks.
- Classifying ASL alphabet gestures (A-Z).
- Performing real-time gesture recognition.
- Supporting accessibility and inclusive communication.

---

## 📂 Dataset

The dataset used in this project was obtained from Roboflow and contains American Sign Language (ASL) alphabet gestures for the 26 English letters.

### 🔗 Dataset Link

[ASL Sign Language Dataset on Roboflow](https://universe.roboflow.com/pbdiplomodv/sign_language-m2nvf/dataset/1)

### Dataset Information

- Number of Classes: 26
- Labels: A-Z
- Annotation Format: YOLO
- Source: Roboflow Universe
- Purpose: Hand Gesture Recognition and ASL Classification

### Class Labels

```text
A B C D E F G H I J K L M
N O P Q R S T U V W X Y Z
```

---

## 📁 Project Structure

```text
├── ai-powered-american-sign-language-asl1-learning.ipynb
│   ├── Dataset Exploration
│   ├── Data Preprocessing
│   ├── Data Augmentation
│   └── Initial Training

├── ai-powered-american-sign-language-asl2-learning.ipynb
│   ├── Hand Landmark Extraction
│   ├── Model Optimization
│   ├── Evaluation
│   └── Deployment Preparation

├── best.pt
│   └── Best YOLO Model

├── best_float16.tflite
│   └── TensorFlow Lite Model (FP16)

├── best_float32.tflite
│   └── TensorFlow Lite Model (FP32)

├── labels.txt
│   └── ASL Alphabet Labels (A-Z)

├── assets
│   ├── dataset_samples.png
│   ├── augmentation.png
│   ├── landmarks.png
│   ├── model_architecture.png
│   ├── yolo_detection.png
│   ├── confusion_matrix.png
│   └── performance_metrics.png

└── README.md
```

---

## 🧩 Phase 1: Dataset Collection & Exploration

### Overview

The project uses an American Sign Language (ASL) alphabet dataset consisting of 26 classes representing the English alphabet letters from A to Z.

### Key Tasks

- Dataset collection and organization.
- Class distribution analysis.
- Data visualization and exploration.
- Image quality inspection.
- Dataset balancing verification.

### Dataset Characteristics

- 26 gesture classes.
- Different backgrounds and lighting conditions.
- Multiple hand orientations.
- Real-world gesture variations.

### Sample Dataset

![Dataset Samples](assets/dataset_samples.png)

---

## 🔄 Phase 2: Data Augmentation

### Overview

Data augmentation was applied to increase dataset diversity and improve model generalization.

### Augmentation Techniques

- Rotation
- Translation
- Scaling
- Brightness Adjustment
- Noise Injection
- Random Transformations

### Benefits

- Reduces overfitting.
- Improves robustness.
- Enhances real-world performance.
- Increases dataset variability.

### Augmentation Example

![Augmentation Example](assets/augmentation.png)

---

## ✋ Phase 3: Hand Detection & Landmark Extraction

### Overview

MediaPipe Hands was used to detect hands and extract 21 hand landmarks for feature representation.

### Processing Pipeline

1. Raw Image Acquisition
2. Image Resizing
3. Hand Detection
4. Landmark Extraction
5. Coordinate Normalization
6. Feature Generation
7. Model Input Preparation

### Extracted Features

- Finger positions
- Finger angles
- Relative landmark distances
- Hand orientation
- Spatial relationships

### Landmark Extraction Example

![Landmark Extraction](assets/landmarks.png)

---

## 🧠 Phase 4: Deep Learning Model Development

### Overview

A deep learning classification model was developed to recognize all ASL alphabet gestures.

### Recognized Classes

```text
A B C D E F G H I J K L M
N O P Q R S T U V W X Y Z
```

### Classification Pipeline

```text
Preprocessed Data
        ↓
Feature Extraction
        ↓
Deep Learning Model
        ↓
Softmax Output Layer
        ↓
Predicted Gesture
```

### Model Architecture

![Model Architecture](assets/model_architecture.png)

### Model Features

- Multi-class classification.
- Optimized for real-time inference.
- Lightweight architecture.
- High recognition accuracy.

---

## 🎯 Phase 5: YOLO-Based Gesture Detection

### Overview

YOLO was trained to detect and classify ASL gestures in real time.

### Advantages

- Fast detection speed.
- Real-time performance.
- Lightweight deployment.
- High localization accuracy.

### Detection Example

![YOLO Detection](assets/yolo_detection.png)

---

## 📊 Phase 6: Model Evaluation

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Results

| Metric | Value |
|----------|----------|
| Validation Accuracy | 89.17% |
| Inference Speed | 189 FPS |
| Model Size | 18 MB |
| Parameters | 4 Million |
| Classes | 26 |

### Confusion Matrix

![Confusion Matrix](assets/confusion_matrix.png)

### Performance Metrics

![Performance Metrics](assets/performance_metrics.png)

### Performance Highlights

- High classification accuracy across 26 classes.
- Fast inference suitable for real-time applications.
- Lightweight model for deployment on edge devices.
- Robust performance under varying conditions.

---

## 🚀 Deployment

The trained model was exported into multiple deployment formats:

### YOLO Model

```text
best.pt
```

### TensorFlow Lite Models

```text
best_float16.tflite
best_float32.tflite
```

### Supported Platforms

- Desktop Applications
- Mobile Devices
- Embedded Systems
- Edge AI Devices
- Real-Time Vision Applications

---

## 🛠️ Technologies Used

- Python 🐍
- OpenCV
- MediaPipe
- YOLOv8
- TensorFlow Lite
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📈 Results Summary

| Metric | Value |
|----------|----------|
| Classes | 26 |
| Accuracy | 89.17% |
| FPS | 189 |
| Model Size | 18 MB |
| Parameters | 4M |
| Deployment Formats | PT, TFLite |

---

## 🚀 How to Run

### Clone Repository

```bash
git clone https://https://github.com/AbdelrahmanMohamed75/Ishara-AI-APP-for-Sign-Language-

cd Ishara-AI-APP-for-Sign-Language-
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Jupyter Notebooks

```bash
jupyter notebook
```

### Run Inference

```bash
python predict.py
```

---

## 🔮 Future Improvements

- Real-time webcam recognition.
- Sentence generation from multiple gestures.
- Arabic Sign Language support.
- Mobile application deployment.
- Transformer-based gesture recognition.
- Continuous sign language recognition.

---

## 👨‍💻 Author

**Abdelrahman Mohamed Emam , Mostafa Sayed Salah**

Faculty of Computer Science and Artificial Intelligence

Data Science | Machine Learning | Computer Vision

---

⭐ If you found this project useful, please consider giving it a Star on GitHub.
