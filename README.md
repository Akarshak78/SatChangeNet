# SatChangeNet

SatChangeNet is a Siamese attention-based deep learning framework for satellite image change detection in remote sensing and smart city monitoring.

## Overview

SatChangeNet is designed for bi-temporal satellite image change detection. The framework combines a shared Siamese ResNet18 encoder with temporal attention, multi-scale feature fusion, and a U-Net-based decoder to identify changes between two satellite images acquired at different times.

## Architecture

The proposed framework consists of:

- Shared Siamese ResNet18 encoder
- Temporal Attention Module (TAM)
- Multi-scale feature fusion
- U-Net decoder
- BCE + Dice loss

## Dataset

The experiments were conducted using the LEVIR-CD dataset.

The dataset is not redistributed in this repository. Please obtain the dataset from its original source and follow the dataset's terms of use.

## Training Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Learning Rate | 1e-4 |
| Batch Size | 8 |
| Epochs | 37 |
| Loss Function | BCE + Dice |
| Scheduler | Cosine Annealing |
| Weight Decay | 1e-4 |
| Image Size | 256 × 256 |

## Environment

The experiments were conducted using:

- Python 3.10
- PyTorch
- CUDA
- NVIDIA Tesla T4 GPU
- Google Colab

### Dataset Path

The notebook uses Google Drive for dataset storage.
Before running the experiments, update the dataset path variables
in the notebook according to the location of the LEVIR-CD dataset
in your own Google Drive.
