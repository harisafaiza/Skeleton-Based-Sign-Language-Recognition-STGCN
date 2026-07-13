# Skeleton-Based-Sign-Language-Recognition-STGCN
A robust skeleton-based sign language recognition framework using Random Forest and Spatio-Temporal Graph Convolutional Networks (ST-GCN) with robustness evaluation under noisy conditions.


# Skeleton-Based Sign Language Recognition Using Spatio-Temporal Graph Convolutional Networks

## Overview

This repository contains the implementation developed as part of my Master's research titled:

**"Skeleton-Based Sign Language Recognition Using Spatio-Temporal Graph Convolutional Networks: A Robustness Analysis."**

The project investigates skeleton-based sign language recognition using both traditional machine learning and deep learning approaches.

The study evaluates:

- Random Forest classifier
- Spatio-Temporal Graph Convolutional Network (ST-GCN)

using pose-based and holistic skeletal representations extracted from sign language videos.

In addition, the robustness of both models is analyzed under different levels of Gaussian noise to understand their behavior in real-world noisy environments.

---

## Research Objectives

The objectives of this research are:

- Develop a skeleton-based sign language recognition pipeline.
- Compare Random Forest and ST-GCN for isolated sign recognition.
- Evaluate pose-only and holistic skeletal features.
- Analyze robustness under noisy conditions.
- Compare performance on benchmark sign language datasets.

---

## Datasets

This project uses the following publicly available datasets:

### LSA64

- 64 isolated Argentinian Sign Language signs
- Used for model training and robustness evaluation

### WLASL

- Large-scale American Sign Language dataset
- Used to evaluate generalization on a more challenging dataset

Dataset links are not included due to licensing restrictions. Please download them from their official sources.

---

## Methodology

The overall pipeline consists of:

1. Video acquisition
2. Frame extraction
3. Skeleton extraction using MediaPipe/OpenPose
4. Pose and holistic feature generation
5. Data preprocessing
6. Model training
7. Performance evaluation
8. Robustness analysis using Gaussian noise

---

## Models

### Random Forest

Traditional machine learning classifier trained on flattened skeleton features.

### ST-GCN

Deep learning model that models both spatial and temporal relationships between skeleton joints using graph convolution.

---

## Feature Types

### Pose Features

- Body keypoints
- Lightweight representation
- Computationally efficient

### Holistic Features

Includes

- Pose
- Face
- Left hand
- Right hand

Provides richer feature representation for sign language recognition.

---

## Experimental Evaluation

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Robustness was evaluated under multiple Gaussian noise levels.

---

## Results

The experiments demonstrate:

- ST-GCN consistently outperforms Random Forest on skeleton sequence modeling.
- Holistic features improve recognition of subtle hand movements.
- Performance degrades under increasing noise, highlighting the importance of robust feature extraction.
- ST-GCN exhibits better robustness than Random Forest in noisy environments.

---

## Repository Structure
project/
│
├── dataset/
├── preprocessing/
├── feature_extraction/
├── models/
│ ├── random_forest/
│ └── stgcn/
├── training/
├── evaluation/
├── results/
├── notebooks/
├── utils/
├── README.md
└── requirements.txt

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Skeleton-Based-Sign-Language-Recognition-STGCN.git

cd Skeleton-Based-Sign-Language-Recognition-STGCN

pip install -r requirements.txt
```
---

##Required Libraries

Python 3.10+

PyTorch

NumPy

OpenCV

MediaPipe

Scikit-learn

Matplotlib

Seaborn

Pandas

Torchvision

Running the Project

Feature Extraction

python extract_features.py

Train Random Forest

python train_rf.py

Train ST-GCN

python train_stgcn.py

Evaluate

python evaluate.py

Research Contributions
1. Skeleton-based sign language recognition framework
2. Comparative study of Random Forest and ST-GCN
3. Pose vs holistic feature comparison
4. Robustness analysis under Gaussian noise
5. Performance evaluation on LSA64 and WLASL datasets

Future Work
Potential extensions include:
1. Real-time sign language recognition
2. Transformer-based architectures
3. Adaptive graph neural networks
4. Improved noise modeling using realistic pose estimation errors
5. Feature selection for facial landmarks to improve efficiency
6. Continuous sign language recognition

Citation

Harisa Faiza Dudekula.

Skeleton-Based Sign Language Recognition Using Spatio-Temporal Graph Convolutional Networks: A Robustness Analysis.

Master of Engineering in Data Science and Artificial Intelligence

Asian Institute of Technology

2026

Acknowledgements
I would like to sincerely thank my advisor, Dr. Chantri Polprasert, for his continuous guidance, encouragement, and valuable insights throughout this research. I also extend my gratitude to the examination committee for their constructive feedback, which helped improve the quality of this work.

License
This project is released for academic and research purposes.
Please cite the original work if you use this repository.
#sign-language-recognition
#computer-vision
#deep-learning
#machine-learning
#graph-neural-networks
#stgcn
#random-forest
#openpose
#action-recognition
#skeleton-based-action-recognition
#python
#pytorch
#artificial-intelligence
#data-science
