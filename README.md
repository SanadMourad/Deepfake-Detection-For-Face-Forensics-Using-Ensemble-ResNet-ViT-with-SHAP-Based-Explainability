# Deepfake Detection for Face Forensics Using Ensemble ResNet-ViT with SHAP-Based Explainability

## Overview

This repository contains the full implementation of the deepfake detection framework presented in the paper:

**"Deepfake Detection for Face Forensics Using Ensemble ResNet-ViT with SHAP-Based Explainability"**  
Submitted to [18th ICCSIT ACM], 2025.

Our approach integrates a convolutional backbone (ResNet-50) and a Vision Transformer (ViT-B16) in a soft-voting ensemble to classify real versus AI-generated facial images. To ensure interpretability, we apply SHAP (SHapley Additive exPlanations) to ResNet-50 outputs, providing pixel-level visual explanations that highlight important facial regions.

## Highlights

- Ensemble of ResNet-50 and ViT-B16 models
- Balanced dataset from Kaggle (5,000 real / 5,000 fake images)
- Stratified train/val/test split (70/15/15)
- SHAP-based explanation pipeline applied to ResNet-50
- Achieved 95.54% test accuracy on the ensemble
- Visual heatmaps of SHAP values for forensic validation

## Dataset

We use the publicly available **200K Real vs AI Visuals** dataset by Muhammad Bilal on Kaggle:

> [https://www.kaggle.com/datasets/muhammadbilal6305/200k-real-vs-ai-visuals-by-mbilal](https://www.kaggle.com/datasets/muhammadbilal6305/200k-real-vs-ai-visuals-by-mbilal)

Only a subset of 10,000 images (5,000 real, 5,000 fake) is used for this study.

