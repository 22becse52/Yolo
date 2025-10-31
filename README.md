# Real-Time **Chain Snatching Detection** using **YOLOv8**

 A deep learning-based surveillance project for detecting **chain-snatching incidents** in **real-time CCTV footage** using **YOLOv8**.

---

## **Project Overview**

Traditional CCTV monitoring depends heavily on human observation, which can lead to **missed incidents** and **delayed responses**.  
This project presents an **automated chain-snatching detection system** powered by **YOLOv8**, capable of identifying **persons**, **bikes/scooters**, and **chain snatchers** directly from surveillance footage.

**Key Capabilities**
- Real-time CCTV-based detection
- Fine-tuned YOLOv8s model with high accuracy
- Detects multiple classes: *person*, *bikes/scooter*, *chain snatcher*
- Ready for deployment on both GPU and CPU systems

---

## **Features**

| Feature | Description |
|----------|-------------|
| Deep Learning | YOLOv8 small (anchor-free) architecture |
| Video Analysis | Detects chain-snatching events from CCTV footage |
| Accuracy | 92.6% mAP@50 overall performance |
| Fine-tuning | Optimized with Adam optimizer for better generalization |
| Lightweight | Runs in real-time on GPU/CPU |
| Dataset | Custom-annotated CCTV dataset (Roboflow) |



##  **Project Structure**
```
 ChainSnatching-Detection/
├──  yolov8_runs/ # Training runs & model weights
│ ├── chain-snatching-exp14/ # Base training results
│ └── chain-snatching-finetune-small/ # Fine-tuned weights (best.pt)
│
├──  results/ # Output screenshots, logs, metrics
├── inference_results/ # Annotated inference videos
│
├── data.yaml # Dataset configuration
├── train.py # Base training script
├── finetune.py # Fine-tuning with advanced params
├── inference.py # Inference on unseen videos
├── requirements.txt # Dependencies list
└── README.md # Project documentation

```

##  **Installation**

Clone the repo and install dependencies:

```bash
git clone https://github.com/22becse52/Yolo/blob/main/yolotraining%20(3).ipynb
cd ChainSnatching-Detection
pip install -r requirements.txt
```

ultralytics
opencv-python
numpy
torch
roboflow


🧠 Model Architecture

Model: YOLOv8s (Small Variant)
Layers: 129  Parameters: 11.1M  GFLOPs: 28.7

🔹 Backbone: CSPDarknet with C2f blocks
🔹 Neck: PANet for feature fusion
🔹 Head: YOLO Detection head (anchor-free)




Results Summary

Real-time detection from CCTV footage
92.6% mAP@50 accuracy
Fine-tuned YOLOv8s model
Efficient inference and robust generalization
