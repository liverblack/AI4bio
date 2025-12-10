# AI4Bio: Artificial Intelligence in Biology & Medicine

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C.svg?style=flat&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Status](https://img.shields.io/badge/Status-Educational-yellow)](https://github.com/liverblack/AI4bio)

## 📖 Introduction

This repository contains a collection of projects and assignments exploring the application of **Artificial Intelligence** and **Deep Learning** in biological and medical contexts. The projects cover three major domains:
1.  **Single-Cell Omics**: Transcriptome analysis and cell typing.
2.  **Medical Imaging**: Ultrasound image classification and segmentation.
3.  **Genomics**: Sequence modeling for translation efficiency prediction.

## 📂 Project Overview

### 🧬 Part 1: Single-Cell RNA-Seq Analysis
*Exploratory Data Analysis and Cell Type Classification on PBMC datasets.*

#### [Project 1: Classical Machine Learning Approach](./Homework1_scRNA_ML.ipynb)
* **Goal**: Classify cell types based on gene expression data.
* **Methods**:
    * **Preprocessing**: Dimensionality reduction using **PCA** and **t-SNE**.
    * **Models**: Logistic Regression, SVM, Random Forest, and k-Nearest Neighbors (kNN).
    * **Results**: Random Forest achieved the most robust performance with high F1-scores across major cell types (CD4 T, CD8 T).

#### [Project 2: Deep Learning & Autoencoders](./Homework2_scRNA_DL.ipynb)
* **Goal**: Advanced dimensionality reduction and classification using Neural Networks.
* **Methods**:
    * **Autoencoder**: Implemented for non-linear dimensionality reduction and latent space visualization.
    * **Architectures**: Compared **Base NN**, **DeepBN** (Batch Norm), **Wide NN**, and **ResNet**.
    * **Optimization**: Analyzed the stability and convergence of SGD vs. AdamW optimizers.

---

### 🏥 Part 2: Medical Image Analysis
*Computer Vision for Breast Cancer Diagnosis.*

#### [Project 3: Breast Ultrasound (BUSI) Analysis](./homework3-overlay.torch.ipynb)
* **Goal**: Automate the diagnosis and segmentation of breast tumors.
* **Dataset**: Breast Ultrasound Images (BUSI) Dataset.
* **Tasks**:
    1.  **Classification**: Fine-tuned **ResNet-101** to classify images as *Normal, Benign, or Malignant*.
    2.  **Segmentation**: Implemented **Attention U-Net** to generate precise masks for tumor regions.
* **Insights**: Evaluated the trade-off between aggressive data cleaning and model generalization capabilities.

---

### 🧬 Part 3: Genomic Sequence Modeling
*Predicting Protein Translation Efficiency.*

#### [Project 4: 5' UTR Sequence Modeling](./homework5_Genomics_CNN.ipynb)
* **Goal**: Predict Mean Ribosome Load (MRL) from 5' UTR DNA sequences.
* **Model**: **1D Convolutional Neural Network (CNN)**.
* **Features**: The model extracts motif features from 50bp sequences to predict translation efficiency.
* **Performance**: Achieved a **Pearson correlation > 0.96** between predicted and actual translation efficiency, validating the model's ability to capture sequence-function relationships.

---

## 🛠️ Technologies & Tools

* **Core**: `Python`, `Jupyter Notebook`
* **Deep Learning**: `PyTorch`, `Torchvision`
* **Machine Learning**: `Scikit-learn`
* **Data Manipulation**: `Pandas`, `NumPy`
* **Visualization**: `Matplotlib`, `Seaborn`

## 🚀 Getting Started

To run these notebooks locally:

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/liverblack/AI4bio.git](https://github.com/liverblack/AI4bio.git)
    cd AI4bio
    ```

2.  **Install dependencies**:
    ```bash
    pip install torch torchvision pandas numpy scikit-learn matplotlib seaborn scipy
    ```

3.  **Run Jupyter Lab**:
    ```bash
    jupyter lab
    ```

