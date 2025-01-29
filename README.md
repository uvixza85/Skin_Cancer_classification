# Skin Cancer Classification using EfficientNet

## Overview

This project implements a deep-learning model for **skin cancer classification** using the **HAM10000 dataset**. The model leverages **EfficientNet** to classify images into **seven different types of skin cancer**. To achieve high classification accuracy, a combination of image normalization, class balancing with Random Oversampling, and hyperparameter tuning using 5-fold Cross-Validation is employed.

## Dataset

The dataset used for this project is **HAM10000**, which contains images of seven different skin cancer types:

1. Actinic keratoses and intraepithelial carcinoma (akiec)
2. Basal cell carcinoma (bcc)
3. Benign keratosis-like lesions (bkl)
4. Dermatofibroma (df)
5. Melanoma (mel)
6. Melanocytic nevi (nv)
7. Vascular lesions (vasc)

## Methodology

1. **Data Preprocessing**

   - Images are **normalized** to ensure uniform input distribution.
   - **Random Oversampling** is applied to address class imbalance.

2. **Model Selection**

   - **EfficientNet** is chosen for feature extraction and classification due to its efficiency and high performance.

3. **Hyperparameter Tuning**

   - A **5-Fold Cross-Validation (CV)** strategy is used to find the best hyperparameters.

4. **Training & Evaluation**

   - The model is trained using the preprocessed dataset.
   - Accuracy is calculated for each fold, and the final performance is averaged.

## Results

| Fold | Accuracy |
| ---- | -------- |
| 1    | 98.52%   |
| 2    | 98.84%   |
| 3    | 98.73%   |
| 4    | 98.41%   |
| 5    | 98.69%   |

**Average Accuracy:** **98.64% ± 0.15%**\
**Best Model Accuracy:** **98.84% (Fold 2)**



