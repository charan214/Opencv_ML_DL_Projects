# 🎥 Real-Time BGR Color Detection using OpenCV

This project is a real-time color detection system that filters and highlights **Blue**, **Green**, or **Red** intensity levels from a live webcam feed. Built with **Python** and **OpenCV**, it uses interactive **trackbars** to dynamically adjust color intensity ranges, allowing users to visually isolate specific BGR components.

---

## 📌 Project Overview

In this project, a webcam is used to:
- Continuously capture video frames.
- Split the image into its **Blue**, **Green**, and **Red** channels.
- Apply **threshold-based masks** for each channel based on values selected using trackbars.
- Combine the masks to isolate the desired color range.
- Display the result in real-time alongside the original image.

This project serves as a fundamental building block for:
- Color-based object detection
- Background subtraction
- Image preprocessing for machine learning and vision models

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV**
- **NumPy**
- **Exploratory Data Analysis (EDA)** for understanding pixel distributions

---

## 📷 Output

- Two windows are shown during execution:
  - **Original Video Feed**
  - **Masked Output**, where only selected BGR intensity ranges are visible.

![demo_image](path_to_your_demo_image_or_gif.gif) *(Replace with your output screenshot or demo)*

---

## 🔍 How It Works

1. Webcam captures live frames using `cv2.VideoCapture()`.
2. Each frame is split into B, G, R channels using `cv2.split()`.
3. Trackbars allow users to set lower and upper thresholds for each color.
4. `cv2.inRange()` is used to create masks for each channel.
5. Final mask is created by combining individual masks.
6. The filtered channels are merged back and displayed alongside the original.

---

## ▶️ How to Run

```bash
pip install opencv-python numpy
python bgr_color_tracker.py


