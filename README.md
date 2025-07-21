# 🛰️ Image Segmentation with U-Net on UAV Images

This project demonstrates the use of **U-Net**, a convolutional neural network architecture, for **semantic image segmentation** on UAV (Unmanned Aerial Vehicle) aerial imagery. The main objective is to detect and segment **buildings** from top-view satellite images using deep learning techniques.

---

## 📌 Project Objective

The goal of this project is to:
- Accurately segment buildings in aerial images.
- Perform pixel-wise classification using deep learning.
- Apply U-Net for efficient semantic segmentation.

---

## 🧠 Model Architecture - U-Net

U-Net is a popular encoder-decoder convolutional neural network architecture designed for biomedical image segmentation, and it is highly effective for satellite/aerial imagery tasks as well.

- **Encoder:** Captures context via downsampling.
- **Decoder:** Enables precise localization via upsampling.
- **Skip Connections:** Preserve spatial details by linking encoder and decoder layers.

---

## 📁 Dataset

**Massachusetts Buildings Dataset**
- A collection of high-resolution satellite images (1500x1500 px) and their corresponding building masks.
- Includes over 150 images for training and testing.

📎 [Dataset Source](https://www.cs.toronto.edu/~vmnih/data/)

---

## ⚙️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- OpenCV
- Matplotlib
- Pillow (PIL)
- Google Colab (for training with GPU support)

---

## 🚀 Workflow

1. **Data Preprocessing**
   - Resizing images and masks to 256×256.
   - Normalizing RGB image values.
   - Augmenting data (optional).

2. **Model Building**
   - Implementing the U-Net architecture from scratch.
   - Using sigmoid activation for binary segmentation.

3. **Training**
   - Loss Function: Binary Crossentropy
   - Optimizer: Adam
   - Evaluation Metric: Intersection over Union (IoU)

4. **Prediction & Visualization**
   - Predicting masks for test images.
   - Comparing ground truth with predicted outputs.

---

## 🔍 Evaluation Metrics

- **Accuracy**
- **Binary Cross-Entropy Loss**
- **IoU Score (Jaccard Index)**

---

## 🖼️ Sample Results

| Original Image | Ground Truth | Predicted Mask |
|----------------|--------------|----------------|
| <img width="1182" height="298" alt="image" src="https://github.com/user-attachments/assets/944eb8b6-e0e5-4c3c-9bd7-7f9323032a1b" />

> Replace these with actual screenshots from your project.

---

## 🛠️ Installation

To run this project locally, install the dependencies using:

```bash
pip install -r requirements.txt

