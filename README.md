# 🚗 License Plate Detection using YOLO (Ultralytics)

A high-accuracy **License Plate Detection system** built using the **Ultralytics YOLO object detection framework**.  
The model is fine-tuned on a large-scale license plate dataset and deployed through a simple **Streamlit web application** that supports video-based inference.

---

## 📌 Project Overview

This project focuses on detecting vehicle license plates in images and videos with:
- High precision (very few false positives)
- Strong recall (very few missed plates)
- Tight and accurate bounding boxes
- Real-time inference performance

The model is trained on ~90k labeled images and evaluated using industry-standard object detection metrics.

---

## 🧠 Model Details

- **Architecture:** YOLO (Nano variant)
- **Framework:** Ultralytics YOLO (PyTorch)
- **Task:** Object Detection
- **Classes:** 1 (`License_Plate`)
- **Input Resolution:** 640 × 640
- **Training Epochs:** 10
- **Batch Size:** 32
- **GPU:** NVIDIA Tesla T4
- **Mixed Precision:** Enabled (AMP)

---

## 📊 Training & Evaluation Results

### ✅ Overall Performance
- **Precision:** ~0.99  
- **Recall:** ~0.94  
- **mAP@50:** ~0.97  
- **mAP@50–95:** ~0.70  

These results indicate a **production-ready model** suitable for real-world license plate detection.

---

## 📈 Training Visualizations

The training process is fully documented using Ultralytics-generated plots:

### 🔹 Confusion Matrix
- Shows clear separation between **License Plate** and **Background**
- Very low false positives
- Strong true positive rate  
✔ Indicates excellent class discrimination

### 🔹 Precision / Recall / F1 / PR Curves
- **Precision Curve:** High precision across confidence thresholds

---<img width="2250" height="1500" alt="BoxP_curve" src="https://github.com/user-attachments/assets/01e86357-eb5c-4bb0-8501-7ab9ad0d161f" />
  
- **Recall Curve:** Stable recall with minimal drop-off
  
<img width="2250" height="1500" alt="BoxR_curve" src="https://github.com/user-attachments/assets/040fd091-ed1d-407c-9690-51d8c1a05bac" />

- **F1 Curve:** Strong balance between precision and recall
  
<img width="2250" height="1500" alt="BoxF1_curve" src="https://github.com/user-attachments/assets/b16f4d5d-17b5-4d2e-b9c9-14101508efd6" />

- **PR Curve:** Large area under curve → robust detector
  
<img width="2250" height="1500" alt="BoxPR_curve" src="https://github.com/user-attachments/assets/f507d18d-aae1-4e93-98e6-3aaef6cf70d4" />

✔ Confirms stable and reliable predictions

---

### 🔹 Train Batch Visualizations
- Annotated samples from training batches
- Demonstrates correct bounding box alignment
- Confirms label integrity and augmentation quality

![train_batch0](https://github.com/user-attachments/assets/49a0a931-c55e-4305-a7d6-5d31bd10fd83)

---

### 🔹 Validation Batch Visualizations
- Model predictions on unseen validation images
- Accurate localization of plates
- Minimal background noise detections

---![val_batch0_labels](https://github.com/user-attachments/assets/b8eade2f-85fd-4ecc-b914-13ccfddf0ed4)

### 🔹 Results & Metrics Plots
Includes:
- Box loss
- Classification loss
- DFL loss
- Precision & Recall per epoch
- mAP@50 and mAP@50–95 trends

✔ All losses decrease smoothly  
✔ Validation metrics improve consistently  
✔ No signs of overfitting

<img width="2400" height="1200" alt="results" src="https://github.com/user-attachments/assets/94252bdc-dd31-4891-b9f4-f338ae68672a" />

---

## 🌐 Streamlit Web Application

A lightweight web interface allows users to:
1. Upload a video
2. Automatically run license plate detection
3. View the processed output with bounding boxes

The detection starts **immediately upon upload** for a smooth user experience.

---

## 🗂 Project Structure

