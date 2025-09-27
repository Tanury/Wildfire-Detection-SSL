# 🔥 WildFire vs No-WildFire Classification with Self-Supervised Learning (SSL)

This project demonstrates **Self-Supervised Learning (SSL) for Computer Vision** using the **Fire/No-Fire image dataset**.  
We first train a ResNet18 backbone with **SimCLR (contrastive pretraining)**, and then fine-tune it for **binary classification**: fire 🔥 vs no-fire 🌲.

---

## 🚀 Features
- Self-Supervised pretraining with **SimCLR**
- Fine-tuning on labeled Fire/No-Fire dataset
- Model evaluation with:
  - Accuracy, Precision, Recall, F1-score
  - ROC Curve & AUC
  - Per-class performance
- Explainability with **Grad-CAM heatmaps**
- Error analysis with **misclassified image visualization**

---

## 📂 Project Structure
FireNoFire_SSL/
|- dataset/ # Fire and No-Fire images
|- models/ # Saved models/checkpoints
|- notebook.ipynb # Main Colab notebook
|- utils.py # Helper functions
|- README.md # Project documentation

---

## 🧠 Training Workflow
1. Self-Supervised Pretraining (SimCLR)
      - Contrastive learning on unlabeled dataset
      - Learns robust visual representations
2. Supervised Fine-Tuning
      - Freeze/unfreeze ResNet backbone
      - Train classifier head for Fire/No-Fire
3. Evaluation & Explainability
      - Compute metrics: accuracy, precision, recall, F1, ROC-AUC
      - Generate confusion matrix
      - Visualize Grad-CAM heatmaps
      - Inspect misclassified images
