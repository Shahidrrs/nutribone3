---
title: NutriBone Knee Osteoporosis Classifier
emoji: 🦴
colorFrom: teal
colorTo: blue
sdk: gradio
sdk_version: 4.44.0
app_file: app.py
pinned: false
license: mit
---

# 🦴 NutriBone — Knee Osteoporosis Classification

Deep learning-based classification of knee osteoporosis from X-ray images using an ensemble of 4 pretrained models.

## Classes
- **Normal** — Healthy bone density
- **Osteopenia** — Early bone density loss (pre-osteoporosis stage)
- **Osteoporosis** — Significant bone density loss with high fracture risk

## Model Architecture
- **Ensemble of 4 models**: VGG-19, ResNet50, EfficientNetB0, ResNet50V2
- **Transfer learning** with two-stage fine-tuning
- **Test Time Augmentation (TTA)** for robust predictions
- **Weighted ensemble** with optimized weights per model

## Performance
| Metric | Value |
|--------|-------|
| Test Accuracy (3-class) | 89.46% |
| External Binary Accuracy | 93.01% |
| Osteoporosis Recall | 91% |

## Dataset
Trained on combined Kaggle knee osteoporosis datasets:
- mohamedgobara/multi-class-knee-osteoporosis-x-ray-dataset
- stevepython/osteoporosis-knee-xray-dataset

## Disclaimer
⚠️ This application is for **research and educational purposes only**.
It is NOT a substitute for professional medical diagnosis.
Always consult a qualified medical professional.
