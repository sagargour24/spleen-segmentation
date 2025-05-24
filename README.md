# 🧬 SpleenNET - Deep Learning for Spleen Segmentation in CT Scans

**SpleenNET** is a convolutional neural network-based medical image segmentation model built to detect and isolate the spleen from abdominal CT images. It leverages a U-Net architecture and is trained on 2D slices to perform pixel-wise classification.

---

## 🧠 Project Overview

- **Goal**: Segment spleen regions from CT scan images with high accuracy  
- **Architecture**: U-Net-like CNN with skip connections  
- **Application**: Medical imaging, radiology assistance, organ volume analysis  

---

## 📂 Dataset

- **Input**: 2D axial CT slices (grayscale)  
- **Label**: Binary segmentation masks (1 = spleen, 0 = background)  
- **Source**: Adapted from public datasets (e.g., Medical Segmentation Decathlon)  

> *Note: Raw datasets are not included due to privacy/medical regulations.*

---

## 🏗️ Model Architecture

- **Encoder**: Convolution → BatchNorm → MaxPool  
- **Decoder**: Transposed Convolution + Skip Connections  
- **Loss Function**: Dice Loss + Binary Cross Entropy  
- **Metrics**: Dice Coefficient, IoU, Accuracy  

---

## Training Performance

<!-- 📌 IMAGE PLACEHOLDER: Training curve (loss & IoU) -->

<sub>Replace images/loss_accuracy_curve.png with your actual training performance plot.</sub>

---

## Sample Outputs

<!-- 📌 IMAGE PLACEHOLDER: Mask overlay on CT -->

<sub>Replace images/spleen_segments.png with overlay of predicted vs. ground truth masks on CT image.</sub>

---

## Input|Ground_Truth|Prediction

<!-- 📌 IMAGE PLACEHOLDER: 3-panel comparison -->

<sub>Replace images/spleen_segments_2.png with side-by-side panels showing input CT, ground truth mask, and predicted mask.</sub>

---

## 🛠️ Requirements

```bash
pip install numpy matplotlib opencv-python scikit-image tensorflow
