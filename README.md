# Tea Leaf Disease Detection Using Deep Learning

## Overview

This project focuses on the automated detection and classification of tea leaf diseases using advanced deep learning models. Multiple transformer-based and convolutional neural network architectures were trained and evaluated using Stratified 5-Fold Cross Validation.

The objective is to support early disease identification in tea plantations through AI-powered image classification, helping improve crop monitoring and decision-making.

---

## Disease Classes

The dataset contains images belonging to the following classes:

- Healthy Leaf
- Gray Blight
- Red Spider
- Helopeltis
- Green Mirid Bug

---

## Models Used

The following deep learning architectures were trained and evaluated:

- Vision Transformer (ViT Base)
- Swin Transformer (Swin Base)
- DeiT Base
- ConvNeXt Base

---

## Methodology

### Data Preprocessing

- Image resizing
- Data augmentation using Albumentations
- Dataset balancing using Weighted Random Sampling
- Image normalization

### Training Strategy

- Stratified 5-Fold Cross Validation
- Focal Loss for handling class imbalance
- Early Stopping
- GPU-accelerated training
- Test-Time Augmentation (TTA)

### Ensemble Learning

Predictions from multiple deep learning models were combined using a Stacking Ensemble approach with Logistic Regression as the meta-learner to improve overall classification performance.

---

## Technologies Used

- Python
- PyTorch
- TIMM
- Albumentations
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Dataset

The dataset consists of tea leaf images representing healthy and diseased samples. The complete dataset is approximately 1.02 GB in size and is not included in this repository due to GitHub storage limitations.

Before running the notebook, place the dataset in the following directory:

```text
./teaLeafBDnoAB_healthymodified
```

---

## Project Structure

```text
Tea-Leaf-Disease-Detection/
│
├── Tea_Leaf_Disease_Detection.ipynb
├── README.md
├── requirements.txt
├── .gitignore
│
├── teaLeafBDnoAB_healthymodified/
└── tea_models_kfold/
```

---

## Features

- Deep Learning-based Disease Classification
- Transformer-based Architectures
- Stratified K-Fold Cross Validation
- Class Imbalance Handling
- Focal Loss Implementation
- Test-Time Augmentation
- Stacking Ensemble Learning
- Confidence Interval Estimation
- Automated Model Evaluation

---

## Results

The models were evaluated using Stratified 5-Fold Cross Validation and a Stacking Ensemble framework.

### Key Components

- Vision Transformer (ViT Base)
- Swin Transformer (Swin Base)
- DeiT Base
- ConvNeXt Base
- Test-Time Augmentation (TTA)
- Logistic Regression Meta-Learner
- Focal Loss for Class Imbalance Handling

### Performance Highlights

- Robust disease classification across multiple tea leaf disease categories.
- Improved generalization through Stratified 5-Fold Cross Validation.
- Enhanced prediction stability using Test-Time Augmentation.
- Increased overall performance through Stacking Ensemble Learning.
- Strong performance achieved using transformer-based architectures combined with ensemble techniques.

The combination of transformer-based architectures and ensemble learning demonstrated significant potential for automated tea leaf disease detection in agricultural applications.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Sarwesh-Phuyal/Tea-Leaf-Disease-Detection.git
```

Move into the project directory:

```bash
cd Tea-Leaf-Disease-Detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

1. Place the dataset inside:

```text
./teaLeafBDnoAB_healthymodified
```

2. Open Jupyter Notebook.

3. Run:

```text
Tea_Leaf_Disease_Detection.ipynb
```

4. Train and evaluate the models.

---

## Notes

- The dataset is not included due to its large size.
- Trained model weights are not included in this repository.
- Users can retrain the models using the provided notebook and dataset.
- A GPU is recommended for training transformer-based models.

---

## Acknowledgements

This project was developed as part of academic research on tea leaf disease detection using deep learning techniques.
