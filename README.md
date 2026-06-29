# Edge-Enabled Deepfake and Image Forgery Detection for Real-Time Surveillance Systems

A multi-stage hybrid image forensics system for detecting image manipulation, deepfakes, and AI-generated images in real time. The project combines traditional digital image forensic techniques with deep learning to provide a robust detection pipeline.

---

## Overview

With the rapid advancement of AI image generation tools and image editing software, detecting manipulated images has become increasingly challenging. This project proposes a multi-stage detection framework capable of identifying:

- Authentic Images
- Tampered Images
- Deepfake Images
- AI-Generated Images

The system combines spatial analysis, frequency-domain analysis, and deep learning to improve detection accuracy across different manipulation techniques.

---

## Features

- Noise inconsistency analysis
- Edge artifact detection
- CNN-based forgery classification
- Deepfake detection using facial frequency analysis
- AI-generated image detection
- Weighted score fusion for final prediction

---

## Detection Pipeline

```
Input Image
      │
      ▼
Noise Analysis
      │
      ▼
Edge Artifact Detection
      │
      ▼
CNN Classification (EfficientNet-B0)
      │
      ▼
Deepfake Detection
      │
      ▼
AI-Generated Image Detection
      │
      ▼
Weighted Score Fusion
      │
      ▼
Final Prediction
```

---

## Methodology

### Stage 1 — Noise Inconsistency Analysis

- Residual noise extraction
- Block variance mapping
- Noise inconsistency scoring

---

### Stage 2 — Edge Artifact Detection

- Canny Edge Density
- Laplacian Sharpness
- Sobel Gradient Analysis

---

### Stage 3 — CNN Classification

- EfficientNet-B0
- Transfer Learning
- Fine-tuned on CASIA 2.0 dataset

---

### Stage 4 — Deepfake Detection

- Haar Cascade Face Detection
- FFT Frequency Analysis
- Boundary Blending Detection

---

### Stage 5 — AI Image Detection

- FFT Spectrum Analysis
- DCT Block Uniformity
- Texture Entropy Analysis

---

## Technologies Used

- Python
- OpenCV
- PyTorch
- NumPy
- Matplotlib
- Scikit-learn
- EfficientNet-B0

---

## Dataset

**CASIA 2.0 Image Tampering Dataset**

- Authentic Images: 7,491
- Tampered Images: 5,123

Training subset:
- 4,000 images
- 80:20 train-validation split

---

## Results

### CNN Performance

| Metric | Score |
|---------|-------|
| Accuracy | 83.6% |
| AUC-ROC | 0.923 |
| F1 Score | 0.831 |

### Full Detection Pipeline

| Metric | Score |
|---------|-------|
| Precision | 0.857 |
| Recall | 0.851 |
| F1 Score | 0.854 |
| AUC | 0.912 |

---

## Repository Structure

```
.
├── DIP.ipynb
├── README.md
└── images/
```

---

## Future Work

- Real-time surveillance deployment
- Larger benchmark datasets
- Vision Transformers
- Improved face detection models
- Web application deployment
- Explainable AI visualizations

---
