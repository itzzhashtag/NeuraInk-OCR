<div align="center">
  
# ✨ NeuraInk - OCR

**by [Aniket Chowdhury](mailto:micro.aniket@gmail.com) (aka `#Hashtag`)**
</div>

<div align="center">  
A hybrid handwritten character recognition system using a Convolutional Neural Network (CNN) trained on the EMNIST dataset.
Supports - Brush Drawing and Live Camera Recognition modes.
</div>


![demo](https://user-images.githubusercontent.com/yourusername/yourdemoimage.gif) <!-- Replace with actual GIF or screenshot -->

---
## 📌 Features

- 🖌️ Draw handwritten characters using a brush canvas
- 📷 Use your webcam for real-time handwriting recognition
- 🤖 Trained on **EMNIST ByClass** (62 classes: A-Z, a-z, 0-9)
- 🌗 Brush mode and Cam mode toggle for GUI
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

📁 Model File: `EMNIST_V2_model.h5`

---

## 🛠 Installation

```bash
# Step 1: Clone the repository
git clone https://github.com/yourusername/NeuraInk-OCR.git
cd NeuraInk-OCR

# Step 2: Install dependencies
pip install -r requirements.txt
```
---

## 🧾 Dataset
- EMNIST ByClass
- 814,255 characters, 62 classes (A-Z, a-z, 0-9)

---

## 📚 Files Overview

| File                               | Description               |  
|------------------------------------|---------------------------|
| CNN Model EMNIST Model v2.py       | CNN model training script |
| EMNIST_V2_model.h5                 | Trained CNN model         |
| EMNIST_V2_history.pkl              | Training history          |
| GUI_EMNIST_V2[Cam].py              | GUI + Mode Switcher       |
| requirements.txt                   | Python dependencies       |

---

## 📌 Future Improvements

- 🖍️ Add Eraser tool to brush mode
- 📷 Integrate region selection for more precise camera predictions
- 🔤 Allow user to correct mispredictions and retrain model incrementally
- 🌐 Deploy as a web app using Flask/Streamlit
- 📱 Build a mobile version using Kivy or Flutter
- 🔁 Add handwriting stroke animation replay
- 📦 Add .exe packaging for easy sharing (via PyInstaller)
- 📊 Visualize CNN layer activations for explainability

---

## 👤 Author & Contact

👨 **Name:** Aniket Chowdhury (aka Hashtag)  
📧 **Email:** [micro.aniket@gmail.com](mailto:micro.aniket@gmail.com)  
💼 **LinkedIn:** [itzz-hashtag](https://www.linkedin.com/in/itzz-hashtag/)  
🐙 **GitHub:** [itzzhashtag](https://github.com/itzzhashtag)  
📸 **Instagram:** [@itzz_hashtag](https://instagram.com/itzz_hashtag)

---

## 📜 License

This project is released under **MIT License** — free for personal and educational use.

---

