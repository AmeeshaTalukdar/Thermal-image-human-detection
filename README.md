

---

# Thermal Image Human Detection using YOLOv5

A deep learning–based object detection system for identifying humans in thermal imagery under challenging visibility conditions such as fog, smoke, and night environments. The project leverages YOLOv5 along with image enhancement techniques to improve detection robustness in low-contrast thermal data.

---

## 📌 Overview

Human detection in low-visibility environments is critical for applications such as surveillance, search & rescue, and autonomous systems. Traditional RGB-based vision systems degrade significantly in such conditions.

This project addresses that limitation by:

* Using **thermal imaging data** instead of RGB
* Applying **image enhancement techniques** to improve feature visibility
* Training a **YOLOv5 object detection model** for robust human detection
* Evaluating performance using standard object detection metrics

---

## 🎯 Key Objectives

* Detect humans in thermal images under adverse conditions
* Improve image quality using preprocessing techniques
* Train and evaluate a YOLOv5-based detection model
* Reduce false positives and improve detection reliability

---

## 🧠 Approach

### 1. Data Preparation

* Thermal image dataset collected from open-source repositories
* Images labeled for human detection (bounding boxes)

### 2. Image Preprocessing

To enhance thermal image quality:

* CLAHE (Contrast Limited Adaptive Histogram Equalization)
* Gamma Correction
* HSV-based contrast enhancement
* Noise reduction and normalization

These techniques improve visibility of human silhouettes in low-contrast thermal frames.

---

### 3. Model Architecture

* YOLOv5 (You Only Look Once - v5)
* Single-stage object detection framework
* Optimized for real-time inference and accuracy trade-off

---

### 4. Training Strategy

* Transfer learning using pre-trained YOLOv5 weights
* Fine-tuned on thermal dataset
* Data augmentation applied for robustness

---

## 🛠️ Tech Stack

* Python
* PyTorch
* YOLOv5 (Ultralytics)
* OpenCV
* NumPy
* Matplotlib

---

## 📊 Results

| Metric                   | Performance             |
| ------------------------ | ----------------------- |
| mAP@0.5                  | 92%                     |
| False Positive Reduction | 15%                     |
| Model Type               | YOLOv5                  |
| Task                     | Thermal Human Detection |

The preprocessing pipeline significantly improved detection consistency in low-visibility scenarios.

---

## 🔍 Inference

Run detection on images:

```bash
python detect.py --weights best.pt --source inference/images
```

---

## 🧪 Training

Train the model using YOLOv5:

```bash
python train.py --img 640 --batch 16 --epochs 100 --data data.yaml --weights yolov5s.pt
```

---

## 📂 Project Structure

```bash
├── dataset/
├── preprocessing/
├── training/
├── inference/
├── models/
├── results/
├── detect.py
├── train.py
├── requirements.txt
└── README.md
```

---

## 🚀 Applications

* Smart surveillance systems
* Search and rescue operations
* Autonomous navigation in low-visibility environments
* Security monitoring systems
* Industrial safety systems

---

## 📈 Impact

This project demonstrates how combining thermal imaging with deep learning can significantly improve human detection performance in environments where RGB cameras fail.

Key improvements:

* Better robustness in adverse conditions
* Improved detection stability
* Reduced false positives through preprocessing

---

## 👤 Author

**Ameesha Talukdar**
AI/ML & Computer Vision Enthusiast

GitHub: [https://github.com/ameeshatalukdar](https://github.com/ameeshatalukdar)

---

## 📌 Note

This project is based on YOLOv5 and thermal imaging research. It was developed as part of an AI/ML learning and applied computer vision exploration effort.

---
