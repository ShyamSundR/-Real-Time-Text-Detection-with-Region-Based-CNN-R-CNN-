# -Real-Time-Text-Detection-with-Region-Based-CNN-R-CNN-
# Real-Time Text Detection with Region-Based CNN (R-CNN)

This project implements a real-time text detection system using a fine-tuned Faster R-CNN model on the MS COCO-Text dataset. The goal is to accurately localize text regions in natural scene images by learning robust object detection features.

## 📁 Project Overview

- **Dataset**: Cleaned subset of MS COCO 2014 with added text annotations ([COCO-Text](https://bgshih.github.io/cocotext/))
- **Model**: Pretrained Faster R-CNN (ResNet50-FPN backbone), fine-tuned for 2-class bounding box detection (text vs. background)
- **Task**: Predict bounding boxes over legible machine-printed text regions in diverse urban and indoor settings

## 🔧 Features

- Custom dataset loader for COCO-Text format
- Scaled annotations and box transformations for normalized input
- Fine-tuning using PyTorch with component-wise loss tracking
- Visualization of predicted vs. ground truth boxes (overlayed in blue/red)
- Checkpoint saving, resume training support
- Component loss curve logging and epoch-wise evaluation

## 🧪 Evaluation

Evaluated on holdout images:
- IOU threshold: 0.5+
- Only predictions with confidence > 0.5 considered
- Model converged with final average losses:
  - `loss_classifier`: ~0.117
  - `loss_box_reg`: ~0.223
  - `loss_rpn_box_reg`: ~0.043
rchvision matplotlib opencv-python scikit-image


LINK : < https://drive.google.com/file/d/1WO0WUT_49j3ZzCp2UP8bu8wl4NEsM4cL/view?usp=sharing >
