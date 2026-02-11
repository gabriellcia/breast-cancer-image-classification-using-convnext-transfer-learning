# Breast Cancer Image Classification Using Convnext Transfer Learning
This repository contains a simple implementation of breast cancer histopathology image classification using a ConvNeXt model with transfer learning. It demonstrates how to adapt a pretrained ConvNeXt network to classify breast cancer images using publicly accessible datasets.

The workflow, implemented in Google Colab, covers:
- loading datasets from Google Drive
- preprocessing and augmentation
- customizing the ConvNeXt architecture for this task
- training with transfer learning
   evaluating model performance
The code can also be executed in a local Jupyter Notebook environment if preferred.

📂 Dataset

Due to file size constraints, the image datasets are hosted on Google Drive. You should download or mount these folders before running the notebook, and update paths accordingly.

- BreakHis 200× dataset : https://drive.google.com/drive/folders/1fHrMNHqArqTD9XtANHzNlNDq41q9nxqj?usp=sharing
- BreastCancerImager dataset : https://drive.google.com/drive/folders/1hV7RVMtem8z2GUffm1_T3exBM32qE5zz?usp=sharing

Place the downloaded folders under a structured directory (e.g., data/BreakHis200x and data/BreastCancerImager), or mount your Google Drive in Colab and point the code to those folders.

🧠 Implementation Overview

The notebook includes:

1. Data Preparation
- Loading image files from Drive
- Preprocessing such as resizing and normalization
- Data augmentation for better generalization
  
2. Model Setup
- Initializing a ConvNeXt model with pretrained ImageNet weights
- Modifying the final classifier head for binary/multiclass classification
  
3.Training and Evaluation
- Training with transfer learning
- Monitoring loss and accuracy
- Calculating classification metrics

This project is intended to be a simple, reproducible demonstration suitable for learning and preliminary research.
