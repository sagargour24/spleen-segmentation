# 🧬 SpleenNET - Medical Image Segmentation with Deep Learning

**SpleenNET** is a deep learning-based project for medical image segmentation, specifically focusing on identifying and segmenting the **spleen** in CT scans. This project uses a convolutional neural network (CNN) architecture to process 2D image slices and generate pixel-level predictions.

---

## 🧠 Project Overview

- **Goal**: Accurately segment spleen regions from abdominal CT scan slices
- **Approach**: Use a U-Net-like architecture for semantic segmentation
- **Data**: Preprocessed 2D image slices derived from medical imaging datasets (e.g., LiTS or MSD)

---

## 🏗️ Model Architecture

The architecture is based on a modified **U-Net**, which includes:

- **Encoder**: Sequential convolutional blocks with max pooling
- **Bottleneck**: Dense convolutional layers with dropout
- **Decoder**: Transposed convolutions with skip connections
- **Output Layer**: `sigmoid` or `softmax` activation for binary/multi-class segmentation

---

## 📊 Evaluation Metrics

- **Dice Coefficient**
- **IoU (Intersection-over-Union)**
- **Pixel-wise Accuracy**
- **Loss Function**: Dice Loss or Binary Cross Entropy + Dice

---

## 🗂️ Dataset

- **Input**: 2D CT slices in grayscale
- **Labels**: Binary masks indicating spleen regions
- **Size**: ~512x512 pixels (resized if needed)

> *Dataset not included due to medical data restrictions. Please request access separately or use a public dataset like the Medical Segmentation Decathlon.*

---

## 🛠️ Requirements

```bash
pip install numpy matplotlib opencv-python tensorflow scikit-image
