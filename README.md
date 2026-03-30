# Multi-Modal Forensic Deepfake Detection System

A deepfake detection system that combines spatial and frequency domain analysis
with explainable AI to classify face images as Real or Fake.

## How It Works

The system analyzes face images through two parallel pathways:
- **Spatial domain** — EfficientNet-B0 extracts visual features from RGB channels
- **Frequency domain** — Fast Fourier Transform (FFT) reveals hidden compression
  artifacts invisible to the human eye

Both features are fused and passed through a binary classifier. Grad-CAM heatmaps
highlight exactly which facial regions triggered the detection.

## Features

- Dual-branch spatial + frequency domain architecture
- EfficientNet-B0 backbone (pretrained on ImageNet, modified for 4-channel input)
- Grad-CAM explainability heatmaps
- Confidence scoring
- Interactive Streamlit web demo

## Tech Stack

- Python, PyTorch, Torchvision
- pytorch-grad-cam
- Streamlit
- Scikit-learn

## Author

Muhammad Furqan Rauf — AI-15 Bootcamp, Computer Vision Module

## Deployed Link
https://vulturelike-unprecipitously-jovani.ngrok-free.dev/

