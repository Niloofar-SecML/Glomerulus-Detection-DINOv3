# Glomerulus-Detection-DINOv3
Detection of glomeruli in kidney histopathology using DINOv3
# Glomerulus Detection using DINOv3 + YOLO11s

This project applies knowledge distillation using DINOv3 as the teacher and YOLO11s as the student to detect glomeruli in kidney tissue histopathology images.

## 🔍 Objective

To improve glomerulus detection accuracy using transformer-based features via distillation.

## 📁 Dataset

- Custom dataset of kidney glomeruli.
- Annotation format: YOLO
- Structure: `/images/train`, `/labels/train`

## 🚀 Method

- Distillation: `dinov3/vits16` → `ultralytics/yolo11s`
- Framework: [`lightly-train`](https://github.com/lightly-ai/lightly-train)

## 🧠 Training Code

All training steps are included in `notebooks/training_pipeline.ipynb`.

## 📦 Installation

```bash
pip install "lightly-train[ultralytics]" "supervision==0.25.1"
