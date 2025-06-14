# ✨ NeuraInk - OCR

> A hybrid handwritten character recognition system using a Convolutional Neural Network (CNN) trained on the EMNIST dataset. Supports **Brush Drawing** and **Live Camera Recognition** modes.

---

![demo](https://user-images.githubusercontent.com/yourusername/yourdemoimage.gif) <!-- Replace with actual GIF or screenshot -->

## 📌 Features

- 🖌️ Draw handwritten characters using a brush canvas
- 📷 Use your webcam for real-time handwriting recognition
- 🤖 Trained on **EMNIST ByClass** (62 classes: A-Z, a-z, 0-9)
- 🌗 Light/Dark mode toggle for GUI
- 💾 Save your drawn image
- ⏹️ Seamlessly switch between modes using the GUI and keyboard

---

## 🎥 Modes

| Mode      | Description                                      | Trigger                     |
|-----------|--------------------------------------------------|-----------------------------|
| Brush     | Default mode - draw and predict characters       | Open app                    |
| Camera    | Webcam-based real-time prediction                | Click `Camera (Testing)`    |
| Exit Cam  | Go back to brush mode                            | Press `Spacebar`            |

---

## 🧠 Model Architecture

- 3x Conv2D Layers with increasing filters
- Batch Normalization & Dropout
- Dense layer (512 units) with L2 Regularization
- Final layer: Softmax (62 output classes)
- Optimizer: Adam with learning rate scheduling

📁 Model File: `emnist_byclass_cnn_model_v2.h5`

---

## 🛠 Installation

```bash
# Step 1: Clone the repository
git clone https://github.com/yourusername/DualMode-EMNIST.git
cd DualMode-EMNIST

# Step 2: Install dependencies
pip install -r requirements.txt
