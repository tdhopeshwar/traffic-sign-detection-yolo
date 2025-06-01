# 🚦 YOLOv11 Traffic Sign Detection

This repository contains a complete training, evaluation, and inference pipeline for detecting 255 types of traffic signs using **YOLOv11**, developed as part of a **private Kaggle competition**. The goal is to improve detection accuracy over baseline YOLOv8 and evaluate model robustness across a diverse range of traffic sign classes.

> ⚠️ **Note**: This project was developed within the scope of a **private Kaggle competition**. The dataset used is not publicly distributed. Please ensure you have appropriate access before attempting to reproduce results.

---

## 📁 Dataset

The dataset consists of:
- `train/images` and `train/labels` – used for training
- `valid/images` and `valid/labels` – used for validation
- `test/images` – used for inference

All annotations follow the YOLO format, and the class list is defined in the `data.yaml` file with 255 traffic sign categories.

---

## 📦 Repository Structure

| File / Folder                  | Description                                                      |
|-------------------------------|------------------------------------------------------------------|
| `yolov11_detection_pipeline.ipynb` | Complete pipeline for training, evaluation, and inference    |
| `data.yaml`                   | Contains dataset configuration and class mappings                |
| `predictions.csv`            | Predicted class names per image                                  |
| `predictions_with_bboxes.csv`| Bounding box outputs with confidence scores                      |
| `images/`                    | Folder for storing visual outputs of model predictions           |

---

## ⚙️ Setup

### 1. Install Dependencies
```bash
pip install ultralytics
