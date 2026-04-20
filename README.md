# 🛒 Retail Shelf Monitoring using Computer Vision

## 📌 Overview

This project implements a **Retail Shelf Monitoring System** using both **traditional computer vision techniques** and **deep learning (YOLOv8)**.

The system analyzes shelf images to:

* Extract visual features
* Compare shelf arrangements
* Detect objects
* Evaluate clutter levels
* Provide structured output for analysis

---

## 🎯 Objectives

* Preprocess shelf images
* Extract features using **HOG** and **SIFT**
* Compare shelf with reference image
* Perform object detection using **YOLOv8**
* Evaluate detection results
* Analyze shelf clutter

---

## 🧠 Methodology

### 🔹 Part I – Traditional Computer Vision

1. **Preprocessing**

   * Grayscale conversion
   * Gaussian blur
   * Histogram equalization

2. **Feature Extraction**

   * **HOG (Histogram of Oriented Gradients)**
   * **SIFT (Scale-Invariant Feature Transform)**

3. **Shelf Comparison**

   * Feature matching using **Brute Force Matcher**
   * Similarity score calculation

---

### 🔹 Part II – Deep Learning

1. **YOLOv8 Object Detection**

   * Pretrained model (`yolov8n.pt`)
   * Low-confidence threshold for detection

2. **Evaluation**

   * Average confidence score
   * Maximum confidence score

3. **Clutter Analysis**

   * Based on number of detected objects:

     * Low
     * Moderate
     * High

---

## ⚙️ Technologies Used

* Python
* OpenCV
* NumPy
* Matplotlib
* Scikit-image
* Ultralytics YOLOv8
* Google Colab

---

## 📂 Project Structure

```
Retail-Shelf-Monitoring/
│── retail_shelf.ipynb
│── main.py
│── README.md
│── images/
│     └── shelf.jpg
```

---

## ▶️ How to Run

1. Open in **Google Colab**
2. Install dependencies:

   ```bash
   pip install ultralytics opencv-python scikit-image matplotlib
   ```
3. Upload shelf image
4. Run all cells

---

## 📊 Output

The system generates:

* Preprocessed image
* HOG feature visualization
* SIFT keypoints
* YOLO detection output
* Structured analysis report

---

## ⚠️ Limitations

* YOLOv8 is trained on **COCO dataset**, which does not include most retail products
* Detection accuracy may be low for shelf items
* Custom dataset training is recommended for real-world applications

---

## 🚀 Future Improvements

* Train YOLO on custom retail dataset
* Real-time shelf monitoring using webcam
* Automatic missing product detection
* Integration with inventory systems

---

## ✅ Conclusion

This project demonstrates how **traditional feature extraction** and **deep learning** can be combined for retail shelf monitoring. While pretrained models have limitations, the system provides a strong foundation for intelligent retail analytics.

---

## 👤 Author

* Dyapa Aravind Reddy

---
