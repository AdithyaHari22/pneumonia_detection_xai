Pneumonia Detection With Spatial Attention and Clinical Metadata

This project implements a deep learning model for pneumonia detection from chest X-rays, incorporating clinical metadata and a spatial attention mechanism to improve interpretability and robustness.

The model uses:

A custom CNN backbone for image feature extraction

Spatial attention to highlight relevant lung regions

A metadata branch (Age, Sex, View position) processed via dense layers

Fusion of image features and metadata for final prediction

BCEWithLogitsLoss with class-balanced weights

Early stopping and learning rate scheduling

Spatial attention heatmaps for model explainability (XAI)

Dataset format and training paths are configured for Google Colab with Google Drive integration.

Key Features

Multimodal Inputs: X-ray + clinical metadata (Age, Sex, AP/PA)

Attention-based CNN: Learns spatial focus areas in the lung

Balanced training: Class-balanced loss for imbalanced medical data

Early stopping + LR scheduler: Stable convergence

Evaluation: Accuracy, Precision, Recall, AUC

XAI: Spatial attention visualization overlay on chest X-rays

Reproducibility: Manual seeds set for PyTorch, NumPy, and CUDA

Acknowledgements

Stanford CheXpert dataset

PyTorch ecosystem

Google Colab + Drive