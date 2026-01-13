# Flower Species Classification using Transfer Learning

## Objective
The goal of this project is to build a high-performance image classifier for 5 flower species (Daisy, Dandelion, Roses, Sunflowers, Tulips) by adapting a pre-trained **ResNet50** model.

## Core Requirements Satisfied:
- **Two-Phase Training:** 1. **Phase 1 (Feature Extraction):** Frozen ResNet50 base with a custom Dense head.
  2. **Phase 2 (Fine-Tuning):** Unfrozen top 10 layers with a low learning rate ($10^{-5}$).
- **Baseline Comparison:** A simple CNN was trained from scratch to quantify the benefits of transfer learning.
- **Model Interpretability:** Implemented **Grad-CAM** to visualize which flower features (petals, centers) the model used for predictions.

## Performance Analysis
- **Confusion Matrix:** The model shows high precision for 'Dandelion' but occasionally confuses 'Roses' and 'Tulips' due to color similarities.
- **Interpretation:** Grad-CAM heatmaps confirm the model focuses correctly on the floral structures rather than background noise.

## Technical Stack
- **Framework:** TensorFlow/Keras
- **Architecture:** ResNet50

- **Tools:** Jupyter (Google Colab), Matplotlib, Scikit-Learn, Seaborn.

## 💾 Model Weights
Due to GitHub's file size limits, the trained ResNet50 model (`best_model.keras`) is hosted on Google Drive.
[Download Model Weights Here]
(https://drive.google.com/file/d/1_ccjgdXf69yCDirXJsRF2FZJdmJloSoy/view?usp=sharing)
