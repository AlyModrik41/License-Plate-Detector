# 🚗 License Plate Detection System

A real-time **license plate detection** application built using **YOLO (Ultralytics)** and **Streamlit**.  
The model is fine-tuned on a custom license plate dataset and can accurately detect license plates in **images and videos** with fast inference speeds.

---

## ✨ Features
- License plate detection using a fine-tuned YOLO model  
- Video upload and processing through a simple web interface  
- Real-time inference with bounding box visualization  
- High accuracy and low latency  
- Easy to extend with OCR or tracking  

---

## 🧠 Model Details
- Base model: **YOLOv8 (pretrained on COCO)**
- Fine-tuned on a custom **license plate dataset**
- Metrics:
  - **mAP@50:** ~95%
  - **Precision:** ~94%
  - **Recall:** ~89%
- Inference speed: ~2–3 ms per image (GPU)

---

## 📁 Project Structure
license_plate_app/
├── app.py # Streamlit application
├── best.pt # Trained YOLO model weights
├── requirements.txt # Dependencies
└── README.md

---

## 🚀 Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/license-plate-detection.git
cd license-plate-detection

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the Streamlit app
streamlit run app.py

